# public.pur_prauthorizationlevel

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| prlevelid | integer | nextval('pur_prauthorizationlevel_prlevelid_seq'::regclass) | false |  |  |  |
| prid | integer |  | true |  |  |  |
| levelid | integer |  | true |  |  |  |
| leveldetailid | integer |  | true |  |  |  |
| ischecked | boolean | false | true |  |  |  |
| formula | varchar(500) |  | true |  |  |  |
| formulavalue | varchar(500) |  | true |  |  |  |
| userid | integer |  | true |  |  |  |
| authorizationlevel | integer |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pur_prauthorizationlevel_pkey | PRIMARY KEY | PRIMARY KEY (prlevelid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pur_prauthorizationlevel_pkey | CREATE UNIQUE INDEX pur_prauthorizationlevel_pkey ON public.pur_prauthorizationlevel USING btree (prlevelid) |

## Relations

![er](public.pur_prauthorizationlevel.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)