# public.prod_batchcardauthorizationlevel

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| batchcardlevelid | integer | nextval('prod_batchcardauthorizationlevel_batchcardlevelid_seq'::regclass) | false |  |  |  |
| batchcardid | integer |  | true |  |  |  |
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
| prod_batchcardauthorizationlevel_pkey | PRIMARY KEY | PRIMARY KEY (batchcardlevelid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| prod_batchcardauthorizationlevel_pkey | CREATE UNIQUE INDEX prod_batchcardauthorizationlevel_pkey ON public.prod_batchcardauthorizationlevel USING btree (batchcardlevelid) |

## Relations

![er](public.prod_batchcardauthorizationlevel.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)