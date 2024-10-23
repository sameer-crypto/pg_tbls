# tmh_service_module.svc_parts_priority

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| svc_priority_id | integer | nextval('tmh_service_module.svc_parts_priority_svc_priority_id_seq'::regclass) | false |  |  |  |
| svc_priority_type_name | varchar(30) |  | true |  |  |  |
| isactive | boolean | true | true |  |  |  |
| inactive_date | date |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | date |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| authorizedon | date |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| edit_log | varchar(50) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| svc_parts_priority_pkey | PRIMARY KEY | PRIMARY KEY (svc_priority_id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| svc_parts_priority_pkey | CREATE UNIQUE INDEX svc_parts_priority_pkey ON tmh_service_module.svc_parts_priority USING btree (svc_priority_id) |

## Relations

![er](tmh_service_module.svc_parts_priority.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)