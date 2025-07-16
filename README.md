# Portfolio-Performance
An accessible repository where field teams can grab customer-facing proof points.

SELECT DISTINCT VersionCr, Avg(ElapsedTime)
FROM iis_log
WHERE Url like '%portfolioview%'
GROUP BY VersionCr
