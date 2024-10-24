# public.set_imp_setting_grp_master

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| groupid | integer | nextval('set_imp_setting_grp_master_groupid_seq'::regclass) | false |  |  |  |
| groupname | varchar(100) |  | true |  |  |  |
| isactive | boolean | false | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| set_imp_setting_grp_master_pkey | PRIMARY KEY | PRIMARY KEY (groupid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| set_imp_setting_grp_master_pkey | CREATE UNIQUE INDEX set_imp_setting_grp_master_pkey ON public.set_imp_setting_grp_master USING btree (groupid) |
| unique_groupname | CREATE UNIQUE INDEX unique_groupname ON public.set_imp_setting_grp_master USING btree (lower((groupname)::text)) |

## Relations

![er](public.set_imp_setting_grp_master.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
