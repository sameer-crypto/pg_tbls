# public.hr_emplanguagedetails

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| emplanguageid | integer | nextval('hr_emplanguagedetails_emplanguageid_seq'::regclass) | false |  |  |  |
| languageid | integer |  | true |  |  |  |
| fluency | varchar |  | true |  |  |  |
| ability | varchar |  | true |  |  |  |
| ondate | timestamp without time zone | now() | true |  |  |  |
| employeeid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| hr_emplanguagedetails_pkey | PRIMARY KEY | PRIMARY KEY (emplanguageid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| hr_emplanguagedetails_pkey | CREATE UNIQUE INDEX hr_emplanguagedetails_pkey ON public.hr_emplanguagedetails USING btree (emplanguageid) |

## Relations

![er](public.hr_emplanguagedetails.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)