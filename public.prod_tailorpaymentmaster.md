# public.prod_tailorpaymentmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| tailorpaymentid | integer | nextval('prod_tailorpaymentmaster_tailorpaymentid_seq'::regclass) | false |  |  |  |
| tailorpaymentno | varchar(50) |  | true |  |  |  |
| productiondate | timestamp without time zone |  | true |  |  |  |
| seriescode | varchar(50) |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| prod_tailorpaymentmaster_pkey | PRIMARY KEY | PRIMARY KEY (tailorpaymentid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| prod_tailorpaymentmaster_pkey | CREATE UNIQUE INDEX prod_tailorpaymentmaster_pkey ON public.prod_tailorpaymentmaster USING btree (tailorpaymentid) |

## Relations

![er](public.prod_tailorpaymentmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)