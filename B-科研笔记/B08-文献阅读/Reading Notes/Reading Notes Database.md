---

database-plugin: basic

---

```yaml:dbfolder
name: new database
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
    isHidden: false
    sortIndex: -1
    position: 1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
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
    isHidden: true
    sortIndex: -1
    position: 2
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
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
    isHidden: true
    sortIndex: -1
    position: 3
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
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
    isHidden: true
    sortIndex: -1
    position: 4
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
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
    isHidden: true
    sortIndex: -1
    position: 5
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
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
    isHidden: true
    sortIndex: -1
    position: 6
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
  Authors:
    input: text
    accessorKey: Authors
    key: Authors
    id: Authors
    label: Authors
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
  PDFAttachments:
    input: text
    accessorKey: PDFAttachments
    key: PDFAttachments
    id: PDFAttachments
    label: PDFAttachments
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
  rating:
    input: select
    accessorKey: rating
    key: rating
    id: rating
    label: rating
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "🍓", backgroundColor: "hsl(306, 95%, 90%)"}
      - { label: "🍓🍓", backgroundColor: "hsl(251, 95%, 90%)"}
      - { label: "🍓🍓🍓", backgroundColor: "hsl(67, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "2D materials,Raman", backgroundColor: "hsl(204, 95%, 90%)"}
      - { label: "Raman", backgroundColor: "hsl(271, 95%, 90%)"}
      - { label: "2D materials", backgroundColor: "hsl(262, 95%, 90%)"}
      - { label: "quantum Hall effect", backgroundColor: "hsl(234, 95%, 90%)"}
      - { label: "graphene", backgroundColor: "hsl(39, 95%, 90%)"}
      - { label: "qutaum Hall effect", backgroundColor: "hsl(172, 95%, 90%)"}
      - { label: "#Electronic-properties-and-materials", backgroundColor: "hsl(198, 95%, 90%)"}
      - { label: "#🍉🍉🍉", backgroundColor: "hsl(347, 95%, 90%)"}
      - { label: "维客笔记", backgroundColor: "hsl(257, 95%, 90%)"}
      - { label: "superconductivity", backgroundColor: "hsl(80, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      wrap_content: true
  Comments:
    input: text
    accessorKey: Comments
    key: Comments
    id: Comments
    label: Comments
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      wrap_content: true
  status:
    input: checkbox
    accessorKey: status
    key: status
    id: status
    label: status
    position: 100
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
config:
  remove_field_when_delete_column: true
  cell_size: wide
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: true
  hoist_files_with_empty_attributes: true
  show_metadata_created: true
  show_metadata_modified: true
  show_metadata_tasks: true
  show_metadata_inlinks: true
  show_metadata_outlinks: true
  source_data: current_folder
  source_form_result: root
  source_destination_path: /
  frontmatter_quote_wrap: false
  row_templates_folder: /
  current_row_template: 
  pagination_size: 10
  enable_js_formulas: true
  formula_folder_path: /
  inline_default: false
  inline_new_position: top
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
filters:
  enabled: false
  conditions:
```