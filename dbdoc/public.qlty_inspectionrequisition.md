# public.qlty_inspectionrequisition

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| reqid | integer | nextval('qlty_inspectionrequisition_reqid_seq'::regclass) | false |  |  |  |
| reqno | varchar |  | true |  |  |  |
| reqdate | date |  | true |  |  |  |
| sourceid | integer |  | true |  |  |  |
| issourcestage | boolean |  | true |  |  |  |
| reqby | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| iscancelled | boolean |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| isauthorized | boolean |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesno | varchar(20) |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| qlty_inspectionrequisition_pkey | PRIMARY KEY | PRIMARY KEY (reqid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| qlty_inspectionrequisition_pkey | CREATE UNIQUE INDEX qlty_inspectionrequisition_pkey ON public.qlty_inspectionrequisition USING btree (reqid) |

## Relations

![er](public.qlty_inspectionrequisition.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
