# public.fa_insurancemaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| insuranceid | integer | nextval('fa_insurancemaster_insuranceid_seq'::regclass) | false |  |  |  |
| insuranceno | varchar(50) |  | true |  |  |  |
| vendorid | integer |  | true |  |  |  |
| annualpremium | numeric(14,4) |  | true |  |  |  |
| startdate | date |  | true |  |  |  |
| enddate | date |  | true |  |  |  |
| policycoverage | numeric(14,4) |  | true |  |  |  |
| policyno | varchar(30) |  | true |  |  |  |
| dateofpurchase | date |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| iscancelled | boolean | false | false |  |  |  |
| seriesno | integer |  | true |  |  |  |
| seriescode | varchar(50) |  | true |  |  |  |
| insurancetypeid | integer |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| glid | integer |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| fa_Insurancemaster_pkey | PRIMARY KEY | PRIMARY KEY (insuranceid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| fa_Insurancemaster_pkey | CREATE UNIQUE INDEX "fa_Insurancemaster_pkey" ON public.fa_insurancemaster USING btree (insuranceid) |

## Relations

![er](public.fa_insurancemaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)