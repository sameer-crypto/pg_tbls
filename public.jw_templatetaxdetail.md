# public.jw_templatetaxdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| taxdetailid | integer | nextval('jw_templatetaxdetail_taxdetailid_seq'::regclass) | false |  |  |  |
| jobworkid | integer |  | true |  |  |  |
| taxid | integer |  | true |  |  |  |
| rate | numeric(5,2) |  | true |  |  |  |
| taxtemplateid | integer |  | true |  |  |  |
| taxtemplatedetailid | integer |  | true |  |  |  |
| taxformula | varchar(150) |  | true |  |  |  |
| taxformulavalue | varchar(150) |  | true |  |  |  |
| taxamount | numeric(12,2) | 0 | true |  |  |  |
| taxorder | integer |  | true |  |  |  |
| asperactual | boolean | false | true |  |  |  |
| exporttaxamount | numeric(17,5) | NULL::numeric | true |  |  |  |
| dutyhead | integer |  | true |  |  |  |
| payabletoparty | boolean | false | true |  |  |  |
| formula_on | numeric(17,5) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| jw_templatetaxdetail_taxdetailid_pkey | PRIMARY KEY | PRIMARY KEY (taxdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| jw_templatetaxdetail_taxdetailid_pkey | CREATE UNIQUE INDEX jw_templatetaxdetail_taxdetailid_pkey ON public.jw_templatetaxdetail USING btree (taxdetailid) |

## Relations

![er](public.jw_templatetaxdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)