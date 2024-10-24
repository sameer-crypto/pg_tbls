# public.sale_discount_slab_master

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| slab_id | integer | nextval('sale_discount_slab_master_slab_id_seq'::regclass) | false |  |  |  |
| slab_code | varchar(100) | NULL::character varying | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| slab_name | varchar |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| seriescode | varchar |  | true |  |  |  |
| remark | varchar |  | true |  |  |  |
| isfreescheme | boolean | false | true |  |  |  |
| isitemgroupwise | boolean | false | false |  |  |  |
| isattributewise | boolean | false | false |  |  |  |
| attributeid | integer | 0 | false |  |  |  |
| isrebate | boolean | false | true |  |  |  |
| iscumulativeqty | boolean | false | true |  |  |  |
| formid | integer | 0 | false |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_discount_slab_master_pkey | PRIMARY KEY | PRIMARY KEY (slab_id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_discount_slab_master_pkey | CREATE UNIQUE INDEX sale_discount_slab_master_pkey ON public.sale_discount_slab_master USING btree (slab_id) |

## Relations

![er](public.sale_discount_slab_master.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
