# public.comn_dmsurlconfiguration

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| tableid | integer | nextval('comn_dmsurlconfiguration_tableid_seq'::regclass) | false |  |  |  |
| urlcode | varchar(50) |  | true |  |  |  |
| urldesc | text |  | true |  |  |  |
| isactive | boolean | false | true |  |  |  |
| requestmethod | varchar(20) |  | true |  |  |  |
| lastsyncdate | timestamp(6) without time zone | now() | true |  |  |  |
| isusedummyapi | boolean | true | true |  |  |  |
| dummyurl | text |  | true |  |  |  |
| istokenenabled | boolean | false | true |  |  |  |
| tokenurl | text |  | true |  |  |  |
| tokenuserid | varchar(50) |  | true |  |  |  |
| tokenpassword | varchar(100) |  | true |  |  |  |
| last_alterid | integer | 0 | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| comn_dmsurlconfiguration_pkey | PRIMARY KEY | PRIMARY KEY (tableid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| comn_dmsurlconfiguration_pkey | CREATE UNIQUE INDEX comn_dmsurlconfiguration_pkey ON public.comn_dmsurlconfiguration USING btree (tableid) |

## Relations

![er](public.comn_dmsurlconfiguration.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
