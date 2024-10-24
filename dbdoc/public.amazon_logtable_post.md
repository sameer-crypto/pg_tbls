# public.amazon_logtable_post

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| plogid | integer | nextval('amazon_logtable_post_plogid_seq'::regclass) | false |  |  |  |
| pdate | date |  | true |  |  |  |
| ptime | varchar(20) |  | true |  |  |  |
| feed | varchar(20) |  | true |  |  |  |
| feed_type | varchar(50) |  | true |  |  |  |
| from_date | timestamp(6) without time zone |  | true |  |  |  |
| to_date | timestamp(6) without time zone |  | true |  |  |  |
| submitted_date | timestamp(6) without time zone |  | true |  |  |  |
| requestid | varchar(200) |  | true |  |  |  |
| report_requestid | varchar(200) |  | true |  |  |  |
| generated_reportid | varchar(200) | ''::character varying | true |  |  |  |
| mws_status | text |  | true |  |  |  |
| application_status | text |  | true |  |  |  |
| is_processed | boolean | false | true |  |  |  |
| file_name | varchar(100) | ''::character varying | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pk_amazon_logtable_post | PRIMARY KEY | PRIMARY KEY (plogid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pk_amazon_logtable_post | CREATE UNIQUE INDEX pk_amazon_logtable_post ON public.amazon_logtable_post USING btree (plogid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| trg_clear_log | CREATE TRIGGER trg_clear_log AFTER INSERT OR UPDATE ON public.amazon_logtable_post FOR EACH ROW EXECUTE FUNCTION clear_log() |

## Relations

![er](public.amazon_logtable_post.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
