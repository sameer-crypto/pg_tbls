# tmh_service_module.svc_service_detail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| svc_service_type_detailid | integer | nextval('tmh_service_module.svc_service_detail_svc_service_type_detailid_seq'::regclass) | false |  |  |  |
| svc_service_type_id | integer |  | true |  |  |  |
| svc_sub_service_type | varchar(30) |  | true |  |  |  |
| isinvoiceable | boolean | true | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | date |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| authorizedon | date |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| svc_service_detail_pkey | PRIMARY KEY | PRIMARY KEY (svc_service_type_detailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| svc_service_detail_pkey | CREATE UNIQUE INDEX svc_service_detail_pkey ON tmh_service_module.svc_service_detail USING btree (svc_service_type_detailid) |

## Relations

![er](tmh_service_module.svc_service_detail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
