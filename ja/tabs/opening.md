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
#published: false


# you can always move this content to _data/content/ folder
# just create new file at _data/content/links/[language].yml and move content below.
###########################################################
#                Links Page Data
###########################################################
page_data:
  main:
    header: "配属希望のみなさん"
    info: "荒瀬研では特任研究員を募集しています。また学内・学外を問わず自然言語処理・計算言語学の研究に取り組みたい学部生・大学院生を募集しています。意欲的で好奇心旺盛な方を歓迎しています。 **Note:** 研究生の受け入れはしていません。"

  # To change order of the Categories, simply change order. (you don't need to change list order.)
  category:
    - title: "特任研究員"
      type: id_postdoc
      color: "#6fa8dc"
    - title: "博士課程"
      type: id_phd
      color: "#F4A273"
    - title: "修士課程"
      type: id_master
      color: "#62b462"
    - title: "学部生（学士特定課題研究）"
      type: id_undergrad
      color: "#ea9999"

  list:
    -
    # 特任研究員
    - type: id_postdoc
      title: "医療言語処理"
      info: "医療言語処理プロジェクトで研究員（特任助教・研究院）を募集しています。 興味のある方はレジュメと業績リストとともに荒瀬まで連絡してください。"

    # 博士課程
    - type: id_phd
      title: "国内の大学院を修了（予定）したの方"
      url: "https://educ.titech.ac.jp/cs/admissions/"
      info: "興味のある方はレジュメと業績リスト、研究計画とともに荒瀬まで連絡してください。入試の詳細については情報理工学院の入試案内を参照してください。"

    # Master students
    - type: id_master
      title: "国内の大学を卒業（予定）したの方"
      url: "https://educ.titech.ac.jp/cs/admissions/"
      info: "情報理工学院情報工学系を受験してください。入試の詳細については情報理工学院の入試案内を参照してください。定期的に研究室公開を開催しています。興味のある方は荒瀬まで連絡してください。"

    # Undergraduates
    - type: id_undergrad
      title: "東工大生"
      info: "定期的に研究室公開を開催しています。興味のある方は荒瀬まで連絡してください。"
------
