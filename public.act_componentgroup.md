# public.act_componentgroup

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| componentgroupid | integer | nextval('act_componentgroup_componentgroupid_seq'::regclass) | false |  |  |  |
| groupname | varchar(255) |  | true |  |  |  |
| inactive | boolean | false | true |  |  |  |
| inactivedate | date |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createddate | timestamp(6) without time zone | now() | true |  |  |  |
| updateby | integer |  | true |  |  |  |
| updatedate | timestamp(6) without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| updateremarks | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| act_componentgroup_pkey | PRIMARY KEY | PRIMARY KEY (componentgroupid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| act_componentgroup_pkey | CREATE UNIQUE INDEX act_componentgroup_pkey ON public.act_componentgroup USING btree (componentgroupid) |

## Relations

![er](public.act_componentgroup.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)