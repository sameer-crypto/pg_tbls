# public.comn_reporttemplate

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| templateid | integer | nextval('comn_reporttemplate_templateid_seq'::regclass) | false |  |  |  |
| templatename | varchar(250) |  | true |  |  |  |
| userid | integer |  | true |  |  |  |
| reportid | integer |  | false |  |  |  |
| isdefault | boolean | false | true |  |  |  |
| isactive | boolean | true | false |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| comn_reporttemplate_pkey | PRIMARY KEY | PRIMARY KEY (templateid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| comn_reporttemplate_pkey | CREATE UNIQUE INDEX comn_reporttemplate_pkey ON public.comn_reporttemplate USING btree (templateid) |

## Relations

![er](public.comn_reporttemplate.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
