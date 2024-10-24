# public.pm_preventivemaintenanceactual

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| pmid | integer | nextval('pm_preventivemaintenanceactual_pmid_seq'::regclass) | false |  |  |  |
| pmno | varchar(30) |  | true |  |  |  |
| pmdate | timestamp without time zone |  | true |  |  |  |
| assetid | integer |  | false |  |  |  |
| employeeid | integer |  | false |  |  |  |
| seriesno | integer |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesvouchertype | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
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
| iscancelled | boolean | false | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |
| stageid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| Unique_pmno_pmdate_branch | UNIQUE | UNIQUE (pmno, pmdate, branchid) |
| pm_preventivemaintenanceactual_pkey | PRIMARY KEY | PRIMARY KEY (pmid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| Unique_pmno_pmdate_branch | CREATE UNIQUE INDEX "Unique_pmno_pmdate_branch" ON public.pm_preventivemaintenanceactual USING btree (pmno, pmdate, branchid) |
| pm_preventivemaintenanceactual_pkey | CREATE UNIQUE INDEX pm_preventivemaintenanceactual_pkey ON public.pm_preventivemaintenanceactual USING btree (pmid) |

## Relations

![er](public.pm_preventivemaintenanceactual.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
