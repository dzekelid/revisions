{
  "info": {
    "name": "Instructure Canvas Groups API Show revision",
    "_postman_id": "7e9878f5-a4d2-44a1-bbbd-ea854f518dc6",
    "description": "Show revision.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "4b551a94-55bc-4cbb-a71d-151ce13226a7",
          "name": "create-a-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/groups?description=%7B%7D&is_public=%7B%7D&join_level=%7B%7D&name=%7B%7D&storage_quota_mb=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eefecf95-8896-4282-b33a-dd819fd80ec7"
            }
          ]
        },
        {
          "id": "3ac47681-a9aa-47a6-80f5-a0dbb66bdddb",
          "name": "get-a-single-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a687f2b-4337-4879-8884-7085cfdf82d1"
            }
          ]
        },
        {
          "id": "b6a4d628-d72b-45bd-ac57-74b013f58a8f",
          "name": "edit-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "avatar_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_public",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "join_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "members",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "storage_quota_mb",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b939d009-ed04-4f00-b250-987b3213db0e"
            }
          ]
        },
        {
          "id": "33a47dae-2c42-4ff7-bc7d-ce9285cff258",
          "name": "delete-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5b40303-1c13-4921-b39d-9fb132ec1c42"
            }
          ]
        },
        {
          "id": "88d2cd9c-6ca7-425d-bba8-fe3af4ed2abc",
          "name": "group-activity-stream",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Group activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ab3a62d-e558-45a4-9b18-951e1bafa2e4"
            }
          ]
        },
        {
          "id": "f970684d-35ee-4538-bd97-4f2b7269b277",
          "name": "group-activity-stream-summary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream/summary"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Group activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd4394da-7230-412d-8335-484f865507d6"
            }
          ]
        },
        {
          "id": "10c1139e-eb15-4074-9943-c7acd2ce9f69",
          "name": "redirect-to-the-assignment-override-for-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/assignments/assignment_id/override"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Redirect to the assignment override for a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dd55add-11c9-49be-bf4e-6e182eaa2767"
            }
          ]
        },
        {
          "id": "8d178ac6-809c-40cc-bb4b-fc22733c0c51",
          "name": "list-conferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/conferences"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List conferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1d4a9b9-24f8-4e90-beb7-d0ae0e768260"
            }
          ]
        },
        {
          "id": "d0cdd512-792a-42d1-8c4e-1d95b2cf7ddc",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd5c2bd3-46ca-4487-bf27-1dc1e0a31640"
            }
          ]
        },
        {
          "id": "9ef49588-21dc-4eeb-9ddc-24344c291d9b",
          "name": "export-content",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
              ],
              "query": [
                {
                  "key": "export_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_notifications",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Export content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78645a12-0e44-47e5-a392-c6eba1cafbf9"
            }
          ]
        },
        {
          "id": "6e062510-c7e8-4f56-83df-b293f11a9c84",
          "name": "show-content-export",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show content export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "389418a7-1aec-4ea1-a26f-38e8baaa4886"
            }
          ]
        },
        {
          "id": "b34c4830-3d4a-4308-a833-035799f20106",
          "name": "list-licenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_licenses"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List licenses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a594e6f4-32b6-435b-94c5-4e83dc436baf"
            }
          ]
        },
        {
          "id": "8994de61-d7df-40e0-960f-f8012ffe69ac",
          "name": "list-content-migrations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content migrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44955e2d-d93a-4c64-b7aa-3b7181251abc"
            }
          ]
        },
        {
          "id": "e5d3ea32-1954-4592-91bf-e2965b6ae77c",
          "name": "create-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
              ],
              "query": [
                {
                  "key": "date_shift_options[day_substitutions][X]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[remove_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[shift_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "migration_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[*]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[file_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[folder_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[overwrite_quizzes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[source_course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad666d14-4e76-45c8-acbf-3c73d88a2205"
            }
          ]
        },
        {
          "id": "5e811dd1-65df-4e5d-8813-5dbf8fc7c9e4",
          "name": "list-migration-issues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0c246e3-8d85-42e5-8c85-3ad7d53e6609"
            }
          ]
        },
        {
          "id": "a4e5251e-3ed0-400a-a40c-cd1660a07775",
          "name": "get-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d3bf330-1db4-4805-9680-4648f34433ae"
            }
          ]
        },
        {
          "id": "0e4da8ad-f89d-461b-8d89-0d576789c91c",
          "name": "update-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "query": [
                {
                  "key": "workflow_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e870cdae-489e-4791-84c5-195f6cd9ca79"
            }
          ]
        },
        {
          "id": "18e40fe4-0e08-41b3-bd02-065e056123ef",
          "name": "get-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c1bcc8b-3617-4c3e-be27-6697143ef718"
            }
          ]
        },
        {
          "id": "6e7edd04-2fbb-4d3b-9230-762b83478cff",
          "name": "update-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c512fa3b-73e7-495d-a395-238bf9eff4d2"
            }
          ]
        },
        {
          "id": "d20e7f51-4748-496b-b05f-c261ed4c99ce",
          "name": "list-migration-systems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/migrators"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration systems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a17317a4-3146-4462-8a64-cd762736b655"
            }
          ]
        },
        {
          "id": "d1864f27-427f-4133-a439-4a1b1be694da",
          "name": "list-discussion-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "only_announcements",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List discussion topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e2dda6a-e4fd-47f1-a5c6-cefce31b8106"
            }
          ]
        },
        {
          "id": "2d44a95d-be7f-4c0e-9f46-76911c90da00",
          "name": "create-a-new-discussion-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new discussion topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70ddb2bc-4101-4dd8-b35a-2fa9e2c2c2ac"
            }
          ]
        },
        {
          "id": "9ebc51dd-d9d7-4c90-bb65-03d0826f9bda",
          "name": "reorder-pinned-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/reorder"
              ],
              "query": [
                {
                  "key": "order",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reorder pinned topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5902c9f-a29f-45a3-83bb-1a02f46d2ac6"
            }
          ]
        },
        {
          "id": "96e43ffb-110c-4ca7-8c47-5847b492e842",
          "name": "get-a-single-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41e21712-43fd-4864-b85a-72220eacf3f7"
            }
          ]
        },
        {
          "id": "ee86bc84-f7a1-4f36-93a5-67b6dd14991e",
          "name": "update-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b41fba9-6ca7-4bea-a22d-f2c4e42b71f6"
            }
          ]
        },
        {
          "id": "ccf2cb7f-1e2b-4931-81af-9313a6da7882",
          "name": "delete-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1ace4bc-e03f-4389-afd3-e505d8b8a091"
            }
          ]
        },
        {
          "id": "199eb642-b37b-4537-9665-f60f665edc32",
          "name": "list-topic-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List topic entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73f3707c-29fa-409a-87f3-d30700e596bb"
            }
          ]
        },
        {
          "id": "21dccf8c-f925-4865-9ae0-002a8063c635",
          "name": "post-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5916a58-6d52-4ebd-8ea6-a7a8ae66f5e7"
            }
          ]
        },
        {
          "id": "3b563ab9-1933-4e75-b138-5712def848c0",
          "name": "rate-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/rating"
              ],
              "query": [
                {
                  "key": "rating",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Rate entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89de7fac-3ebc-45b2-a498-4ac6ec366323"
            }
          ]
        },
        {
          "id": "a440d2dd-fcde-4908-9ef2-153e8c0ba4b2",
          "name": "mark-entry-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22dbf3d9-7736-48d0-8903-799c6512c03d"
            }
          ]
        },
        {
          "id": "7232d2a5-0150-4b4f-8258-00209f939e5b",
          "name": "mark-entry-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dcf483c-6746-4181-ab8c-196713e978e9"
            }
          ]
        },
        {
          "id": "dd49380d-106f-4e3c-8c45-aba8553f1ac7",
          "name": "list-entry-replies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List entry replies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a32f08d-e145-4781-9082-af4063727387"
            }
          ]
        },
        {
          "id": "c932797b-c767-4f56-908e-03a6f8fa92c2",
          "name": "post-a-reply",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post a reply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70dee918-9939-41e6-b340-fd639efaa082"
            }
          ]
        },
        {
          "id": "670b667b-2bb8-4f0b-9320-701b9c144601",
          "name": "update-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ec7b96e-8622-4528-a039-4829a61c94f5"
            }
          ]
        },
        {
          "id": "6b6a4468-f178-43fd-b99c-317aac2fb904",
          "name": "delete-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48620f57-13f5-41c8-8041-815ceec212e6"
            }
          ]
        },
        {
          "id": "29399f63-d711-4125-bf96-71acb31f5a25",
          "name": "list-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entry_list"
              ],
              "query": [
                {
                  "key": "ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f619bc47-b446-4563-b627-e9369dfdb2ce"
            }
          ]
        },
        {
          "id": "5c186ac5-4e16-4dc6-aa06-44b25432f45f",
          "name": "mark-topic-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark topic as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c08e0f3-6b13-4827-8346-72b979998b92"
            }
          ]
        },
        {
          "id": "64b745f2-40d5-48f5-8335-2f967b99534b",
          "name": "mark-topic-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark topic as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "354ac119-4057-4ebb-a8f3-0e3364304e2f"
            }
          ]
        },
        {
          "id": "4151484c-f36c-408a-a5e5-de683f62b3e2",
          "name": "mark-all-entries-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all entries as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dce19bf-ce4b-4edc-bc86-b02a0101348c"
            }
          ]
        },
        {
          "id": "7161a635-7b69-489b-bd77-27570f58be0f",
          "name": "mark-all-entries-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all entries as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3e6e14b-6481-4629-a38c-cf1225eabe75"
            }
          ]
        },
        {
          "id": "32b5558e-d6fa-4deb-af73-112c793b2726",
          "name": "subscribe-to-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Subscribe to a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "577a88d0-109f-42a9-b082-75f90656fa72"
            }
          ]
        },
        {
          "id": "2676112d-514e-4171-a385-d1e8f362c592",
          "name": "unsubscribe-from-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unsubscribe from a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bc86959-f694-467f-9ec1-0249e8b6c343"
            }
          ]
        },
        {
          "id": "ff64fa14-b2e7-4bd6-809c-61dcfdfd1d7d",
          "name": "get-the-full-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/view"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the full topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "330a3ebd-a66a-4f7b-aa25-0bd13f9c4236"
            }
          ]
        },
        {
          "id": "3cf3589c-2b2f-452d-a244-07b25e03d6b3",
          "name": "list-external-feeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/external_feeds"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List external feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3a78651-aaa5-4691-a88d-a816c0e1f19e"
            }
          ]
        },
        {
          "id": "866fd55a-4a93-4aa2-a248-2fbaf6443608",
          "name": "create-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/external_feeds"
              ],
              "query": [
                {
                  "key": "header_match",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "verbosity",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "262cdb58-9c8c-494f-abf1-82b8e8227329"
            }
          ]
        },
        {
          "id": "0854f70b-ccf8-4283-b344-7fb6c4447d9c",
          "name": "delete-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/external_feeds/external_feed_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "920a6924-9818-41e0-95ab-44f38b12dca8"
            }
          ]
        },
        {
          "id": "089d6c04-1026-4880-8020-e1b38d5860a0",
          "name": "list-files",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/files"
              ],
              "query": [
                {
                  "key": "content_types",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "only",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6d041b6-beed-4d9a-bff9-996eec639f68"
            }
          ]
        },
        {
          "id": "9d2f8ada-03ec-4fb4-9b1e-fda8bf4f9d67",
          "name": "upload-a-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/files"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45253073-7fa0-47ba-8b3c-f9e5f0d070e2"
            }
          ]
        },
        {
          "id": "ee4f8fe6-ae3e-4a51-8575-3cf9f718e07b",
          "name": "get-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/files/id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Respon