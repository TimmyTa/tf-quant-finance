<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tf_quant_finance.experimental.dates.date_utils.year_month_day_to_ordinal" />
<meta itemprop="path" content="Stable" />
</div>

# tf_quant_finance.experimental.dates.date_utils.year_month_day_to_ordinal

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/google/tf-quant-finance/blob/master/tf_quant_finance/experimental/dates/date_utils.py">View source</a>



Calculates ordinals Tensor given years, months and dates.

```python
tf_quant_finance.experimental.dates.date_utils.year_month_day_to_ordinal(
    year, month, day
)
```



<!-- Placeholder for "Used in" -->


#### Args:


* <b>`year`</b>: Tensor of int32 type. Elements should be positive.
* <b>`month`</b>: Tensor of int32 type of same shape as `year`. Elements should be in
  range `[1, 12]`.
* <b>`day`</b>: Tensor of int32 type of same shape as `year`. Elements should be in
  range `[1, 31]` and represent valid dates together with corresponding
  elements of `month` and `year` Tensors.


#### Returns:

Tensor of int32 type. Each element is number of days since 1 Jan 0001. 1 Jan
0001 has `ordinal = 1`.