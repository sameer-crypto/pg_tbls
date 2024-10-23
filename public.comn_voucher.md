# public.comn_voucher

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| voucherid | integer | nextval('comn_voucher_voucherid_seq'::regclass) | false |  |  |  |
| vouchername | varchar(100) |  | true |  |  |  |
| formid | smallint |  | true |  |  |  |
| isdefault | boolean | false | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| isactive | boolean | false | true |  |  |  |
| branchid | smallint |  | true |  |  |  |
| allowbackdateentry | boolean | false | true |  |  |  |
| bamount_auth_enable | boolean | false | true |  |  |  |
| isinclusivetaxrate | boolean | false | true |  |  |  |
| tallyvouchername | varchar(200) |  | true |  |  |  |
| isitemlevelroundingoff | boolean | false | true |  |  |  |
| isnettotalroundingoff | boolean | false | true |  |  |  |
| item_noofdecimal | smallint | 0 | true |  |  |  |
| forautocreatetransaction | boolean | false | true |  |  | True when It's a default voucher for automatic created transactions. |
| iserpvoucher | boolean | false | true |  |  |  |
| take_effectofpricelist_mrpabatement_in_si | boolean | false | true |  |  |  |
| vouchertype_condition_in_generateseries | boolean | true | true |  |  |  |
| si_used_for_stock_transfer | boolean | false | true |  |  |  |
| si_item_rate_as | smallint | 0 | true |  |  |  |
| get_normal_pi_in_tsi | boolean | false | true |  |  |  |
| isusedforopening | boolean |  | true |  |  |  |
| create_ratediff_cndn_on_invoice | boolean | false | true |  |  |  |
| editlog | text |  | true |  |  |  |
| shortname | varchar(500) |  | true |  |  |  |
| take_effect_in_rg23d | boolean | false | true |  |  |  |
| si_mrp_inclusive_of_dealers_margin | boolean | false | true |  |  | for MDH |
| generate_exciseserialno | boolean | false | true |  |  |  |
| calculate_exicseonmrp | boolean | false | true |  |  |  |
| linkedvoucherid | integer | 0 | true |  |  |  |
| isimeiapplicable | boolean | false | true |  |  |  |
| defaulttaxtemplateid | integer |  | true |  |  |  |
| impact_on_input_classification | boolean | false | true |  |  |  |
| savedatawithoutserial | boolean | false | true |  |  |  |
| transfer_one_store | boolean | false | true |  |  |  |
| default_print_voucher | smallint |  | true |  |  |  |
| pts_ptr_calculation | boolean |  | true |  |  |  |
| istakeimpactpotency | boolean |  | true |  |  |  |
| takeeffectofdplandrebate | boolean | false | true |  |  |  |
| billofsupply | boolean |  | true |  |  |  |
| isbranchtransfer | boolean |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| exclude_from_sales | boolean | false | true |  |  |  |
| not_required_in_tally | boolean | false | true |  |  |  |
| usedforhighseapurchase | boolean | false | false |  |  |  |
| usedforlut | boolean | false | true |  |  |  |
| usedforexportinvoice | boolean | false | true |  |  |  |
| bifurcateqtyobsric | boolean |  | true |  |  |  |
| usedformanualhsnrate | boolean | false | true |  |  |  |
| usedforsocialwelfaretaxes | boolean | false | true |  |  |  |
| hidefromgstrreport | boolean | false | false |  |  |  |
| auto_authorize_on_save | boolean | false | true |  |  |  |
| pick_rate_from | integer | 1 | true |  |  |  |
| issiinvoicewithso | boolean | false | true |  |  |  |
| issiinvoicepurpose | integer | 0 | true |  |  |  |
| istreatasbranchchallan | boolean | false | true |  |  |  |
| isusedforforgingindustry | boolean | false | false |  |  |  |
| dwbnotrequired | boolean |  | true |  |  |  |
| isbatchmrpwithpricediscount | boolean | false | true |  |  |  |
| showallbatchcardofselecteditemincopybatchcard | boolean | false | true |  |  |  |
| isallowsingleorderformarketplace | boolean | false | false |  |  |  |
| skipprprocess | boolean | false | false |  |  |  |
| issubpoapplicable | boolean | false | true |  |  |  |
| is_global_order | boolean | false | true |  |  |  |
| is_proformalinkedwithdn | boolean | false | true |  |  |  |
| is_dlnote_scanning_through_app | boolean | false | true |  |  |  |
| is_grossweightcalculationonbalesdln | boolean | false | true |  |  |  |
| setservicepidatebackuptospo | boolean | false | true |  |  |  |
| isitembominpo | boolean | false | true |  |  |  |
| udf_customization_on_production_scanning_consumebatch | boolean | false | true |  |  |  |
| isdisplaybatchnoinbatchcard | boolean | false | true |  |  |  |
| isbranchtransferinward | boolean | false | true |  |  |  |
| is_serpiwospo | boolean | false | true |  |  |  |
| isfreeschemeimpactindlnwso | boolean | false | true |  |  |  |
| isrcmrequired | boolean | false | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |
| isdharmada | boolean | false | true |  |  |  |
| ispreserialscanning | boolean | false | true |  |  |  |
| tcscalculationon | integer | '-1'::integer | true |  |  |  |
| itemcategoryfilterid | integer | 0 | true |  |  |  |
| isvchasexport | boolean | false | true |  |  |  |
| _preserialscanninginsales | boolean | false | true |  |  |  |
| is_icwopo_against_si | boolean | false | true |  |  |  |
| isnotforic | boolean | false | true |  |  |  |
| displaymultilevelinworkorder | boolean | false | true |  |  |  |
| workorderreferanceinbatchcard | boolean | false | true |  |  |  |
| isgstrequired_alt | boolean | false | true |  |  |  |
| tdscalculationon | integer | 0 | true |  |  |  |
| validatefssai | boolean | false | true |  |  |  |
| issetratezero | boolean | false | true |  |  |  |
| takeimpactofmrpbasedonvoucher | boolean | false | true |  |  |  |
| servicemappedfor | integer |  | true |  |  |  |
| isallowbackdate_nolimit | boolean | false | true |  |  |  |
| usefor_easyecom | boolean | false | true |  |  |  |
| isrgpmerge_rgpinsource | boolean | false | true |  |  |  |
| usefor_expiredbatch_transfer | boolean | false | true |  |  |  |
| isbatteryfeaturemergewithlubricant | boolean | false | true |  |  |  |
| is_poqty_lessthan_bargainqty | boolean | false | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| VoucherAlreadyExist | UNIQUE | UNIQUE (vouchername, formid, branchid) |
| comn_voucher_pkey | PRIMARY KEY | PRIMARY KEY (voucherid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| VoucherAlreadyExist | CREATE UNIQUE INDEX "VoucherAlreadyExist" ON public.comn_voucher USING btree (vouchername, formid, branchid) |
| comn_voucher_pkey | CREATE UNIQUE INDEX comn_voucher_pkey ON public.comn_voucher USING btree (voucherid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| voucher_log_entry() | CREATE TRIGGER "voucher_log_entry()" AFTER UPDATE ON public.comn_voucher FOR EACH ROW EXECUTE FUNCTION voucher_log_entry() |

## Relations

![er](public.comn_voucher.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
