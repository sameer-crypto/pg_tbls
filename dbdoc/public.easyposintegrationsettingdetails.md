# public.easyposintegrationsettingdetails

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| id | bigint | nextval('easyposintegrationsettingdetails_id_seq'::regclass) | false |  |  |  |
| tokenurl | text |  | true |  |  |  |
| tokenkey | text |  | true |  |  |  |
| tokenemailid | text |  | true |  |  |  |
| tokenpassword | text |  | true |  |  |  |
| attributemasurl | text |  | true |  |  |  |
| unitmasurl | text |  | true |  |  |  |
| itemgroupurl | text |  | true |  |  |  |
| itemmasterurl | text |  | true |  |  |  |
| salesinvoiceurl | text |  | true |  |  |  |
| isactive | boolean | true | true |  |  |  |
| createdon | timestamp(6) without time zone | now() | true |  |  |  |
| erpmappingurl | text |  | true |  |  |  |
| servicemappingurl | text |  | true |  |  |  |
| ismrplessabatement | boolean | false | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| easyposintegrationsettingdetails_pkey | PRIMARY KEY | PRIMARY KEY (id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| easyposintegrationsettingdetails_pkey | CREATE UNIQUE INDEX easyposintegrationsettingdetails_pkey ON public.easyposintegrationsettingdetails USING btree (id) |

## Relations

![er](public.easyposintegrationsettingdetails.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
