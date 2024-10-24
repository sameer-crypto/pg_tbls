# importexport.sale_incrementalexportcertificate

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| certificateid | integer | nextval('importexport.sale_incrementalexportcertificate_certificateid_seq'::regclass) | false |  |  |  |
| certificateno | varchar |  | true |  |  |  |
| certificatedate | date |  | true |  |  |  |
| rangefrom | date |  | true |  |  |  |
| rangeto | date |  | true |  |  |  |
| submissiondate | date |  | true |  |  |  |
| authority | varchar |  | true |  |  |  |
| isincrementalexportcostreceived | boolean |  | true |  |  |  |
| receivedamount | numeric(15,5) |  | true |  |  |  |
| receivedno | varchar |  | true |  |  |  |
| receiveddate | date |  | true |  |  |  |
| remarks | text |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| createdby | integer |  | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| iscancelled | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| seriescode | varchar(50) |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| amendby | integer |  | true |  |  |  |
| amendon | date |  | true |  |  |  |
| seriesvouchertype | smallint | 0 | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| amendreason | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_incrementalexportcertificate_pkey | PRIMARY KEY | PRIMARY KEY (certificateid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_incrementalexportcertificate_pkey | CREATE UNIQUE INDEX sale_incrementalexportcertificate_pkey ON importexport.sale_incrementalexportcertificate USING btree (certificateid) |

## Relations

![er](importexport.sale_incrementalexportcertificate.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
