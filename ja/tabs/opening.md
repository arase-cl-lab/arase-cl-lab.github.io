---
layout: opening
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_opening

# publish date (used for seo)
# if not specified, site.time will be used.
#date: 2022-03-03 12:32:00 +0000

# for override items in _data/lang/[language].yml
#title: My title
#button_name: "My button"
# for override side_and_top_nav_buttons in _data/conf/main.yml
#icon: "fa fa-bath"

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-03-03 12:32:00 +0000
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# please use the "image_viewer_on" below to enable image viewer for individual pages or posts (_posts/ or [language]/_posts folders).
# image viewer can be enabled or disabled for all posts using the "image_viewer_posts: true" setting in _data/conf/main.yml.
#image_viewer_on: true
# please use the "image_lazy_loader_on" below to enable image lazy loader for individual pages or posts (_posts/ or [language]/_posts folders).
# image lazy loader can be enabled or disabled for all posts using the "image_lazy_loader_posts: true" setting in _data/conf/main.yml.
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
# published: false


# you can always move this content to _data/content/ folder
# just create new file at _data/content/links/[language].yml and move content below.
###########################################################
#                Links Page Data
###########################################################
page_data:
  main:
    header: "Opening"
    info: "We are recruiting Postdocs and looking for prospective PhD, master, and undergrad students! [Note] We do not have positions for visiting/research students."

  # To change order of the Categories, simply change order. (you don't need to change list order.)
  category:
    - title: "Postdocs"
      type: id_postdoc
      color: "#6fa8dc"
    - title: "PhDs"
      type: id_phd
      color: "#F4A273"
    - title: "Master"
      type: id_master
      color: "#62b462"
    - title: "Undergraduates"
      type: id_undergrad
      color: "#ea9999"

  list:
    -
    # Postdocs
    - type: id_postdoc
      title: "Medical NLP"
      info: "We are looking for a couple of postdocs on the medical NLP project. Please send Yuki Arase your resume and list of publications."

    # PhD students
    - type: id_phd
      title: "International students"
      url: "https://www.titech.ac.jp/english/admissions/prospective-students/graduate-programs/igp"
      info: "We are looking for PhD students highly motivated to advance NLP/CL technplogy. Please send Yuki Arase your resume, list of publications, and research proposal. For details of admission, please visit the TITECH's official addmision page."

    # Master students
    - type: id_master
      title: "International students"
      url: "https://www.titech.ac.jp/english/admissions/prospective-students/graduate-programs/igp"
      info: "We are looking for international students highly motivated to advance NLP/CL technplogy. Please send Yuki Arase your resume, list of publications, and research proposal. For details of admission, please visit the TITECH's official addmision page."

    # Undergraduates
    - type: id_undergrad
      title: "TITECH students"
      info: "We hold online/phisical open lab events. Please contact Yuki Arase for details."
---
