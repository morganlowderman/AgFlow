select pricingmkt, station, comm, deltaqty, contractfreightprice, allinMP, positionmonth, contmonth, VaRCommodityCode, source, *
from vwallpositionsrisk
where comm like '%vessel freight%'
and iscurrent = 'y'
and deltaqty <> 0
and pricingmkt = 'are'
and station = 'alg'
