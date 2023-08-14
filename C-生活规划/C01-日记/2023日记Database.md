---

database-plugin: basic

---

```yaml:dbfolder
name: 2023日记Database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 1
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  __created__:
    key: __created__
    id: __created__
    input: metadata_time
    label: Created
    accessorKey: __created__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: true
    position: 16
    isHidden: false
    sortIndex: 1
    width: 194
    isSorted: true
    isSortedDesc: true
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  __modified__:
    key: __modified__
    id: __modified__
    input: metadata_time
    label: Modified
    accessorKey: __modified__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: true
    position: 2
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  __tasks__:
    key: __tasks__
    id: __tasks__
    input: task
    label: Task
    accessorKey: __tasks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 3
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: false
      footer_type: none
      persist_changes: false
      persist_formula: false
  __inlinks__:
    key: __inlinks__
    id: __inlinks__
    input: inlinks
    label: Inlinks
    accessorKey: __inlinks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 4
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  __outlinks__:
    key: __outlinks__
    id: __outlinks__
    input: outlinks
    label: Outlinks
    accessorKey: __outlinks__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: false
    position: 5
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  反思:
    input: text
    accessorKey: 反思
    key: 反思
    id: 反思
    label: 反思
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 135
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
      wrap_content: true
      content_alignment: text-align-left
  天气:
    input: select
    accessorKey: 天气
    key: 天气
    id: 天气
    label: 天气
    position: 12
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "🌞", backgroundColor: "hsl(122, 95%, 90%)"}
      - { label: "🌤️", backgroundColor: "hsl(264, 95%, 90%)"}
      - { label: "🌧️", backgroundColor: "hsl(339, 95%, 90%)"}
      - { label: "🌨️", backgroundColor: "hsl(6, 95%, 90%)"}
      - { label: "❄️", backgroundColor: "hsl(118, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
      content_alignment: text-align-center
      wrap_content: true
  心情:
    input: select
    accessorKey: 心情
    key: 心情
    id: 心情
    label: 心情
    position: 13
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "😀", backgroundColor: "hsl(52, 95%, 90%)"}
      - { label: "🙂", backgroundColor: "hsl(213, 95%, 90%)"}
      - { label: "😑", backgroundColor: "hsl(238, 95%, 90%)"}
      - { label: "🫤", backgroundColor: "hsl(341, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  要事:
    input: text
    accessorKey: 要事
    key: 要事
    id: 要事
    label: 要事
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 144
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
      wrap_content: true
      content_alignment: text-align-left
      content_vertical_alignment: align-middle
  早起:
    input: select
    accessorKey: 早起
    key: 早起
    id: 早起
    label: 早起
    position: 14
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Y", backgroundColor: "hsl(152,57%,73%)"}
      - { label: "N", backgroundColor: "hsl(228,39%,70%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  早睡:
    input: select
    accessorKey: 早睡
    key: 早睡
    id: 早睡
    label: 早睡
    position: 15
    skipPersist: false
    isHidden: true
    sortIndex: -1
    options:
      - { label: "Y", backgroundColor: "hsl(152,57%,73%)"}
      - { label: "N", backgroundColor: "hsl(228,39%,70%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  日期:
    input: calendar
    accessorKey: 日期
    key: 日期
    id: 日期
    label: 日期
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  随想:
    input: text
    accessorKey: 随想
    key: 随想
    id: 随想
    label: 随想
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 107
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
      wrap_content: true
      content_alignment: text-align-left
  标签:
    input: tags
    accessorKey: 标签
    key: 标签
    id: 标签
    label: 标签
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "obsidian技巧", backgroundColor: "hsl(288, 95%, 90%)"}
      - { label: "软件", backgroundColor: "hsl(211, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
  图片:
    input: text
    accessorKey: 图片
    key: 图片
    id: 图片
    label: 图片
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      persist_formula: false
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: true
  show_metadata_modified: true
  show_metadata_tasks: true
  show_metadata_inlinks: true
  show_metadata_outlinks: true
  source_data: current_folder
  source_form_result: root
  source_destination_path: /
  row_templates_folder: Z-附件/Templates/日记模板
  current_row_template: Z-附件/Templates/日记模板.md
  pagination_size: 200
  font_size: 16
  enable_js_formulas: true
  formula_folder_path: /
  inline_default: false
  inline_new_position: top
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: true
  implementation: default
filters:
  enabled: true
  conditions:
      - condition: AND
        disabled: true
        label: "1月"
        color: "hsl(355,93%,88%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-01"
      - condition: AND
        disabled: true
        label: "2月"
        color: "hsl(267,93%,88%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-02"
      - condition: AND
        disabled: true
        label: "3月"
        color: "hsl(78, 95%, 90%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-03"
      - condition: AND
        disabled: true
        label: "4月"
        color: "hsl(328,93%,88%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-04"
      - condition: AND
        disabled: true
        label: "5月"
        color: "hsl(131, 95%, 90%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-05"
      - condition: AND
        disabled: true
        label: "6月"
        color: "hsl(238,73%,84%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-06"
      - condition: AND
        disabled: true
        label: "7月"
        color: "hsl(214,71%,85%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-07"
      - condition: AND
        disabled: true
        label: "8月"
        color: "hsl(168,93%,88%)"
        filters:
        - field: 反思
          operator: CONTAINS
          value: "2023-08"
      - condition: AND
        disabled: true
        label: "9月"
        color: "hsl(93,74%,85%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-09"
      - condition: AND
        disabled: true
        label: "10月"
        color: "hsl(52,93%,88%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-10"
      - condition: AND
        disabled: true
        label: "11月"
        color: "hsl(279,93%,88%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-11"
      - condition: AND
        disabled: true
        label: "12月"
        color: "hsl(134, 95%, 90%)"
        filters:
        - field: 日期
          operator: CONTAINS
          value: "2023-12"
```