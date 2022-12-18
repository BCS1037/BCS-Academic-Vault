---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: "__file__"
    id: "__file__"
    input: "markdown"
    label: "File"
    accessorKey: "__file__"
    isMetadata: "true"
    skipPersist: "false"
    isDragDisabled: "false"
    csvCandidate: "true"
    config:
      enable_media_view: "true"
      link_alias_enabled: "true"
      media_width: "100"
      media_height: "100"
      isInline: "true"
      task_hide_completed: "true"
  __created__:
    key: "__created__"
    id: "__created__"
    input: "metadata_time"
    label: "Created"
    accessorKey: "__created__"
    isMetadata: "true"
    isDragDisabled: "false"
    skipPersist: "false"
    csvCandidate: "true"
    config:
      enable_media_view: "true"
      link_alias_enabled: "true"
      media_width: "100"
      media_height: "100"
      isInline: "false"
      task_hide_completed: "true"
  __modified__:
    key: "__modified__"
    id: "__modified__"
    input: "metadata_time"
    label: "Modified"
    accessorKey: "__modified__"
    isMetadata: "true"
    isDragDisabled: "false"
    skipPersist: "false"
    csvCandidate: "true"
    config:
      enable_media_view: "true"
      link_alias_enabled: "true"
      media_width: "100"
      media_height: "100"
      isInline: "false"
      task_hide_completed: "true"
  __tasks__:
    key: "__tasks__"
    id: "__tasks__"
    input: "task"
    label: "Task"
    accessorKey: "__tasks__"
    isMetadata: "true"
    isDragDisabled: "false"
    skipPersist: "false"
    csvCandidate: "false"
    config:
      enable_media_view: "true"
      link_alias_enabled: "true"
      media_width: "100"
      media_height: "100"
      isInline: "false"
      task_hide_completed: "true"
  __inlinks__:
    key: "__inlinks__"
    id: "__inlinks__"
    input: "inlinks"
    label: "Inlinks"
    accessorKey: "__inlinks__"
    isMetadata: "true"
    isDragDisabled: "false"
    skipPersist: "false"
    csvCandidate: "false"
    config:
      enable_media_view: "true"
      link_alias_enabled: "true"
      media_width: "100"
      media_height: "100"
      isInline: "false"
      task_hide_completed: "true"
  __outlinks__:
    key: "__outlinks__"
    id: "__outlinks__"
    input: "outlinks"
    label: "Outlinks"
    accessorKey: "__outlinks__"
    isMetadata: "true"
    isDragDisabled: "false"
    skipPersist: "false"
    csvCandidate: "false"
    config:
      enable_media_view: "true"
      link_alias_enabled: "true"
      media_width: "100"
      media_height: "100"
      isInline: "false"
      task_hide_completed: "true"
config:
  remove_field_when_delete_column: "true"
  cell_size: "normal"
  sticky_first_column: "false"
  group_folder_column: 
  remove_empty_folders: "false"
  automatically_group_files: "false"
  hoist_files_with_empty_attributes: "true"
  show_metadata_created: "true"
  show_metadata_modified: "true"
  show_metadata_tasks: "true"
  show_metadata_inlinks: "true"
  show_metadata_outlinks: "true"
  source_data: "current_folder"
  source_form_result: "root"
  source_destination_path: "/"
  frontmatter_quote_wrap: "true"
  row_templates_folder: "/"
  current_row_template: 
  pagination_size: "10"
  enable_js_formulas: "true"
  formula_folder_path: "/"
  inline_default: "true"
  inline_new_position: "top"
  date_format: "yyyy-MM-dd"
  datetime_format: "yyyy-MM-dd HH:mm:ss"
filters:
  enabled: false
  conditions:
```