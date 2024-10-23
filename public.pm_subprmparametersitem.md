# public.pm_subprmparametersitem

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| detailid | integer | nextval('pm_subprmparametersitem_detailid_seq'::regclass) | false |  |  |  |
| parameterid | integer |  | false |  |  |  |
| itemid | integer |  | false |  |  |  |
| editlog | text |  | true |  |  |  |
| checklistid | integer |  | false |  |  |  |
| checklistdetailid | integer |  | false |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pm_subprmparametersitem_pkey | PRIMARY KEY | PRIMARY KEY (detailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pm_subprmparametersitem_pkey | CREATE UNIQUE INDEX pm_subprmparametersitem_pkey ON public.pm_subprmparametersitem USING btree (detailid) |

## Relations

![er](public.pm_subprmparametersitem.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)