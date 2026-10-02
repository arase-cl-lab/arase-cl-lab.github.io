---
# Mr. Green Jekyll Theme (https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
# Copyright (c) 2022 Mr. Green's Workshop https://www.MrGreensWorkshop.com
# Licensed under MIT

layout: default
# publications page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}

{%- assign pub_data = page.page_data | default: site.data.content.publications[lng].page_data -%}

{%- assign pub_container_style = nil -%}
{%- if pub_data.main.img -%}
  {%- capture pub_container_style -%} style="background-image:url('{{ pub_data.main.img }}');" {%- endcapture -%}
{%- elsif pub_data.main.back_color %}
  {%- capture pub_container_style -%} style="background-color:{{ pub_data.main.back_color }};" {%- endcapture -%}
{%- endif %}

<div class="multipurpose-container publications-heading-container" {{ pub_container_style }}>
{%- assign color_style = nil -%}
{%- if pub_data.main.text_color -%}
  {%- capture color_style -%} style="color:{{ pub_data.main.text_color }};" {%-endcapture-%}
{%- endif %}
  <h1 {{ color_style }}>{{ pub_data.main.header | default: "Publications" }}</h1>
  <p {{ color_style }}>{{ pub_data.main.info | default: "No data, check page_data in [language]/tabs/publications.md front matter or _data/content/publications/[language].yml" }}</p>
</div>

{%- comment -%} kept outside the heading container so it can stick to the top while scrolling {%- endcomment -%}
<nav class="publications-nav">
  <div class="multipurpose-button-wrapper">
    {%- for category in pub_data.category %}
      <a href="#{{ category.type }}" role="button" class="multipurpose-button publication-buttons" style="background-color:{{ category.color }};">{{ category.title }}</a>
    {% endfor -%}
  </div>
</nav>

{%- for category in pub_data.category %}
<div class="multipurpose-container publication-container" id="{{ category.type }}" style="border-left-color:{{ category.color }};">
  <h2>{{ category.title }}</h2>
  {%- comment -%} sort the year groups, not the entries, so the order inside a year stays as authored {%- endcomment -%}
  {%- assign items = pub_data.list | where: "type", category.type -%}
  {%- assign year_groups = items | group_by: "year" | sort: "name" | reverse -%}
  <div class="markdown-style">
    {%- for group in year_groups %}
    <h3 class="publication-year">{{ group.name }}</h3>
    <ul class="publication-list">
      {%- for item in group.items %}
      <li>{{ item.cite | markdownify }}</li>
      {%- endfor %}
    </ul>
    {%- endfor %}
  </div>
</div>
{% endfor %}
