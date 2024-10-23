# public.eazyerp_dms_response

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| tableid | integer | nextval('eazyerp_dms_response_tableid_seq'::regclass) | false |  |  |  |
| urlcode | varchar(50) |  | true |  |  |  |
| erpmasterid | integer |  | true |  |  |  |
| authtoken | text |  | true |  |  |  |
| sentjson | text |  | true |  |  |  |
| response | text |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| eazyerp_dms_response_pkey | PRIMARY KEY | PRIMARY KEY (tableid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| eazyerp_dms_response_pkey | CREATE UNIQUE INDEX eazyerp_dms_response_pkey ON public.eazyerp_dms_response USING btree (tableid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| trg_clear_log | CREATE TRIGGER trg_clear_log AFTER INSERT ON public.eazyerp_dms_response FOR EACH ROW EXECUTE FUNCTION clear_log() |

## Relations

![er](public.eazyerp_dms_response.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)