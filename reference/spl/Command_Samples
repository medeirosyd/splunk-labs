| Command | Sample 1 | Sample 2 | Sample 3 | Sample 4 |
|---------|----------|----------|----------|----------|
| abstract | `abstract` | `abstract limit=100` | `abstract terms=50` | `abstract terms=50 summarylen=200` |
| accum | `accum count` | `accum bytes` | `accum total_errors` | `accum count AS running_total` |
| addcoltotals | `addcoltotals` | `addcoltotals fieldname=total` | `addcoltotals labelfield=row total` | `addcoltotals label="TOTAL"` |
| addinfo | `addinfo` | `addinfo type=search` | `addinfo | fields info_*` | `addinfo | table info_min_time info_max_time` |
| addtotals | `addtotals` | `addtotals fieldname=row_total` | `addtotals labelfield=metric` | `addtotals col=true labelfield=metric` |
| analyzefields | `analyzefields status` | `analyzefields action` | `analyzefields purchase_result` | `analyzefields class target=response` |
| anomalies | `anomalies` | `anomalies by host` | `anomalies action=blocked` | `anomalies field=latency` |
| anomalousvalue | `anomalousvalue bytes` | `anomalousvalue duration` | `anomalousvalue cpu` | `anomalousvalue latency pthresh=0.01` |
| anomalydetection | `anomalydetection` | `anomalydetection device_id` | `anomalydetection threshold=0.01` | `anomalydetection action=blocked` |
| append | `append [ search index=main error ]` | `append [ search index=main status=500 ]` | `append [ savedsearch="daily_errors" ]` | `append maxtime=30 [ search index=security action=blocked ]` |
| appendcols | `appendcols [ search index=main | head 5 ]` | `appendcols [ search index=main | stats count BY host ]` | `appendcols [ savedsearch="kpi_hosts" ]` | `appendcols [ search index=a | stats sum(bytes) AS sum_a ]` |
| appendpipe | `appendpipe [ stats count AS total ]` | `appendpipe [ eventstats avg(bytes) AS avg_bytes ]` | `appendpipe [ dedup host ]` | `appendpipe [ stats dc(user) AS distinct_users ]` |
| arules | `arules` | `arules min_support=0.1` | `arules max_rules=50` | `arules min_confidence=0.8` |
| associate | `associate` | `associate maxdist=0.3` | `associate showstr=true` | `associate fieldlist=host,action` |
| autoregress | `autoregress value` | `autoregress value p=1` | `autoregress value p=2` | `autoregress value p=3 future_timespan=2` |
| bin | `bin _time span=1h` | `bin bytes span=1000` | `bin latency span=10` | `bin _time span=1d` |
| bucketdir | `bucketdir filepath` | `bucketdir uri` | `bucketdir path` | `bucketdir file_path maxdepth=3` |
| chart | `chart count BY sourcetype` | `chart avg(bytes) BY host` | `chart count BY status uri` | `chart sum(bytes) OVER _time BY host` |
| cluster | `cluster t=0.8` | `cluster labelonly=true` | `cluster showcount=true` | `cluster t=0.99 field=signature` |
| cofilter | `cofilter host user` | `cofilter src_ip dest_ip` | `cofilter method status` | `cofilter uri status maxrows=20` |
| collect | `collect index=summary` | `collect index=summary sourcetype=summary_app` | `collect index=summary addtime=true` | `collect index=summary marker="daily_rollup"` |
| concurrency | `concurrency duration` | `concurrency duration=duration` | `concurrency duration=duration by host` | `concurrency duration=duration normalized=true` |
| contingency | `contingency host status` | `contingency user action` | `contingency src_ip dest_ip` | `contingency uri status showperc=true` |
| convert | `convert timeformat="%Y-%m-%d" ctime(_time)` | `convert num(bytes)` | `convert dur2sec(duration)` | `convert timeformat="%H:%M" ctime(firstTime)` |
| correlate | `correlate` | `correlate fieldlist=host,action` | `correlate maxdist=0.3` | `correlate showstr=true` |
| datamodel | `datamodel Web Web_Events search` | `datamodel Authentication Auth_Events search` | `datamodel Network Traffic search` | `datamodel Web Web_Events search | stats count BY uri` |
| dbinspect | `| dbinspect index=_internal` | `| dbinspect index=main` | `| dbinspect index=*` | `| dbinspect index=security detail=true` |
| dedup | `dedup host` | `dedup user` | `dedup session_id sortby -_time` | `dedup src_ip dest_ip keepevents=true` |
| delete | `delete` | `delete WHERE status=404` | `delete WHERE tag=to_be_removed` | `delete WHERE _time < relative_time(now(), "-30d")` |
| delta | `delta bytes` | `delta bytes AS diff_bytes` | `delta count AS change_in_count` | `delta latency p=2` |
| diff | `| diff` | `| diff limit=20` | `| diff attributes=host,status` | `| diff showrecs=true` |
| erex | `erex field=fieldname example="error 500"` | `erex field=user example="user=john"` | `erex field=code example="status=404"` | `erex field=ip example="src=10.0.0.1"` |
| eval | `eval total=price*quantity` | `eval full_name=first_name." ".last_name` | `eval is_error=if(status>=500,1,0)` | `eval kb=round(bytes/1024,2)` |
| eventcount | `| eventcount summarize=f` | `| eventcount index=main` | `| eventcount index=*` | `| eventcount index=security summarize=t` |
| eventstats | `eventstats avg(bytes) AS avg_bytes` | `eventstats max(bytes) AS max_bytes BY host` | `eventstats dc(user) AS users BY host` | `eventstats sum(bytes) AS total_bytes` |
| extract | `extract pairdelim="," kvdelim="="` | `extract reload=true` | `extract auto` | `extract pairdelim=" " kvdelim="="` |
| fieldformat | `fieldformat bytes=tostring(bytes,"commas")` | `fieldformat latency=latency." ms"` | `fieldformat pct=round(pct,2)."%'"` | `fieldformat status="HTTP ".status` |
| fields | `fields host sourcetype` | `fields + host user status` | `fields - _raw` | `fields + host,sourcetype,-_raw` |
| fieldsummary | `| fieldsummary` | `| fieldsummary index=main` | `| fieldsummary limit=50` | `| fieldsummary fields="host,source"` |
| filldown | `filldown user` | `filldown host session_id` | `filldown field1 field2` | `filldown` |
| fillnull | `fillnull value=0` | `fillnull value="unknown" user` | `fillnull value="N/A" host session_id` | `fillnull value=0 fields="bytes,duration"` |
| findtypes | `findtypes` | `findtypes index=main` | `findtypes maxtypes=50` | `findtypes maxtotal=100` |
| folderize | `folderize path` | `folderize uri` | `folderize filepath maxdepth=3` | `folderize directory` |
| foreach | `foreach field* [ eval <<FIELD>>=upper(<<FIELD>>) ]` | `foreach num* [ eval <<FIELD>>=round(<<FIELD>>,2) ]` | `foreach status* [ eval <<FIELD>>=tostring(<<FIELD>>) ]` | `foreach ip* [ eval <<FIELD>>=lower(<<FIELD>>) ]` |
| format | `format` | `format "(" "(" " OR " ")"` | `format "[" "[" " AND " "]"` | `format "(" "(" " OR " ")" field=host` |
| from | `| from datamodel:Web.Web_Events` | `| from lookup:city_lookup` | `| from csv:mydata.csv` | `| from search:mysavedsearch` |
| gauge | `gauge value 0 25 50 75 100` | `gauge count 0 10 50 100 200` | `gauge latency 0 100 200 500 1000` | `gauge pct 0 25 50 75 100` |
| gentimes | `| gentimes start=-1d` | `| gentimes start=-7d increment=1d` | `| gentimes start=-24h increment=1h` | `| gentimes start=-1mon increment=1d` |
| geom | `geom geo_field` | `geom geo_field featureIdField=feature_id` | `geom geo_field allfeatures=true` | `geom geo_field globallookup=true` |
| geomfilter | `geomfilter geo_field` | `geomfilter geo_field view=world` | `geomfilter geo_field featureIdField=feature_id` | `geomfilter geo_field region="US"` |
| geostats | `geostats count BY lat,long` | `geostats sum(bytes) BY lat,long` | `geostats dc(user) BY lat,long` | `geostats avg(latency) BY lat,long` |
| head | `head 10` | `head 20` | `head 1` | `head 100` |
| highlight | `highlight error` | `highlight error warning` | `highlight host user` | `highlight term=blocked` |
| history | `| history` | `| history limit=20` | `| history user=myuser` | `| history search="index=main"` |
| iconify | `iconify status` | `iconify severity` | `iconify status severity` | `iconify status label=severity` |
| inputcsv | `| inputcsv myfile.csv` | `| inputcsv myfile.csv | stats count` | `| inputcsv myfile.csv | table *` | `| inputcsv append=t myfile.csv` |
| inputlookup | `| inputlookup mylookup` | `| inputlookup mylookup where status="active"` | `| inputlookup mylookup | stats count BY host` | `| inputlookup mylookup index=myindex` |
| iplocation | `iplocation ip` | `iplocation src_ip` | `iplocation clientip` | `iplocation ip prefix=src_` |
| join | `join user [ search index=main auth ]` | `join host [ search index=inventory ]` | `join type=inner session_id [ search index=sessions ]` | `join max=0 host [ search index=assets ]` |
| kmeans | `kmeans k=3 field=latency` | `kmeans k=5 field=bytes` | `kmeans k=4 fields=bytes,latency` | `kmeans k=3 field=value max_iter=20` |
| kvform | `kvform` | `kvform extract=true` | `kvform field=_raw` | `kvform delim="&"` |
| loadjob | `| loadjob savedsearch="admin:search:daily_errors"` | `| loadjob job_id` | `| loadjob savedsearch="myapp:search:summary"` | `| loadjob jid` |
| localize | `localize` | `localize field=_time` | `localize timespan=1h` | `localize maxtimes=50` |
| localop | `localop` | `localop | stats count` | `localop | search error` | `localop | sort -_time` |
| lookup | `lookup mylookup ip OUTPUTNEW city` | `lookup mylookup user OUTPUT dept` | `lookup mylookup host OUTPUT owner` | `lookup local=t mylookup ip OUTPUTNEW country` |
| makecontinuous | `makecontinuous _time` | `makecontinuous _time span=1h` | `makecontinuous _time pad=true` | `makecontinuous _time periods=48` |
| makemv | `makemv delim="," field=values` | `makemv delim=";" field=tags` | `makemv delim=" " field=words` | `makemv values delim=","` |
| makeresults | `| makeresults` | `| makeresults count=5` | `| makeresults 1` | `| makeresults format=csv` |
| map | `map search="search index=main host=$host$"` | `map maxsearches=10 search="search index=main user=$user$"` | `map search="search index=_internal sourcetype=$sourcetype$"` | `map maxsearches=50 search="search index=security src_ip=$src_ip$"` |
| mcollect | `mcollect index=metrics` | `mcollect index=metrics sourcetype=cpu` | `mcollect index=metrics addtime=true` | `mcollect index=metrics marker="rollup"` |
| metadata | `| metadata type=hosts` | `| metadata type=sourcetypes` | `| metadata type=sources` | `| metadata type=hosts index=main` |
| metasearch | `| metasearch index=_internal` | `| metasearch index=main` | `| metasearch index=* sourcetype=access*` | `| metasearch index=security` |
| meventcollect | `meventcollect index=metrics` | `meventcollect index=metrics sourcetype=cpu` | `meventcollect index=metrics addtime=true` | `meventcollect index=metrics marker="convert"` |
| mpreview | `| mpreview index=metrics` | `| mpreview index=metrics metric_name="cpu.usage"` | `| mpreview index=metrics sourcetype=perf` | `| mpreview index=metrics limit=100` |
| msearch | `| msearch index=metrics` | `| msearch index=metrics metric_name="cpu.usage"` | `| msearch index=metrics sourcetype=perf` | `| msearch index=metrics limit=100` |
| mstats | `| mstats avg(cpu.usage) WHERE index=metrics` | `| mstats sum(bytes) WHERE index=metrics BY host` | `| mstats max(latency) WHERE index=metrics span=1h BY host` | `| mstats p95(latency) WHERE index=metrics BY app` |
| multikv | `multikv` | `multikv fields header=true` | `multikv suppressheader=true` | `multikv fields event_no` |
| multisearch | `multisearch [ search index=main error ] [ search index=main warn ]` | `multisearch [ search index=a ] [ search index=b ]` | `multisearch [ search index=security action=blocked ] [ search index=network ]` | `multisearch [ search index=web ] [ search index=api ]` |
| mvcombine | `mvcombine ip` | `mvcombine delim="," user` | `mvcombine host` | `mvcombine values delim=";"` |
| mvexpand | `mvexpand ip` | `mvexpand user` | `mvexpand values` | `mvexpand tag` |
| nomv | `nomv ip` | `nomv delim="," tag` | `nomv user` | `nomv field=values` |
| outlier | `outlier latency` | `outlier cpu` | `outlier bytes` | `outlier latency threshold=3` |
| outputcsv | `outputcsv results.csv` | `outputcsv append=true results.csv` | `outputcsv limit=0 results.csv` | `outputcsv useutf8=true results.csv` |
| outputlookup | `outputlookup mylookup` | `outputlookup append=t mylookup` | `outputlookup key_field=mykey mylookup` | `outputlookup createinapp=t mylookup` |
| outputtext | `outputtext` | `outputtext limit=100` | `outputtext format=raw` | `outputtext format=xml` |
| overlap | `overlap` | `overlap field=_time` | `overlap max=10` | `overlap normalize=true` |
| pivot | `| pivot Web Web_Events count(Web_Events) BY host` | `| pivot Web Web_Events sum(bytes) BY uri` | `| pivot Authentication Auth_Events count(Auth_Events) BY user` | `| pivot Network Traffic avg(latency) BY dest` |
| predict | `predict bytes` | `predict bytes future_timespan=10` | `predict bytes holdback=10` | `predict bytes future_timespan=5 algorithm=LL` |
| rangemap | `rangemap field=latency` | `rangemap field=latency low=0-100 elevated=101-300 severe=301-1000` | `rangemap field=pct low=0-60 elevated=61-90 severe=91-100` | `rangemap field=cpu crit=90-100` |
| rare | `rare host` | `rare uri` | `rare 10 user` | `rare limit=20 showcount=true dest_ip` |
| redistribute | `redistribute` | `redistribute maxreducers=20` | `redistribute parallel=4` | `redistribute maxinputs=100000` |
| regex | `regex _raw="error"` | `regex uri="^/api/"` | `regex field=user "^[A-Z].*"` | `regex ip="^10\\."` |
| reltime | `eval age=reltime(now()-_time)` | `eval ago=reltime(now()-firstTime)` | `eval diff=reltime(lastTime-firstTime)` | `eval delay=reltime(now()-start_time)` |
| rename | `rename host AS server` | `rename user AS username` | `rename src_ip AS src dest_ip AS dest` | `rename field1 AS "Field 1"` |
| replace | `replace "500" WITH "ERROR" IN status` | `replace "404" WITH "NOT_FOUND" IN status` | `replace "yes" WITH "true" IN flag` | `replace "no" WITH "false" IN flag` |
| require | `require` | `require 1` | `require min=1` | `require comment="must have results"` |
| rest | `| rest /services/server/info` | `| rest /services/authentication/users` | `| rest /services/saved/searches` | `| rest splunk_server=local /services/server/settings` |
| return | `return 10 _time host` | `return $count` | `return 20 user` | `return 5 status uri` |
| reverse | `reverse` | `reverse | head 10` | `reverse | tail 5` | `reverse | sort _time` |
| rex | `rex field=_raw "user=(?<user>\\w+)"` | `rex field=_raw "status=(?<status>\\d+)"` | `rex field=uri "/product/(?<product_id>\\d+)"` | `rex field=_raw max_match=0 "ip=(?<ip>\\d+\\.\\d+\\.\\d+\\.\\d+)"` |
| rtorder | `rtorder` | `rtorder _time` | `rtorder host _time` | `rtorder -_time` |
| savedsearch | `| savedsearch my_savedsearch` | `| savedsearch "daily_errors"` | `| savedsearch app:search:summary` | `| savedsearch "admin:search:baseline"` |
| script | `script myscript` | `script myscript param=value` | `script myscript field=_raw` | `script myscriptqueue=myqueue` |
| scrub | `scrub` | `scrub ip` | `scrub user` | `scrub host` |
| search | `search error` | `search index=main status=500` | `search sourcetype=access_combined` | `search index=security action=blocked` |
| searchtxn | `searchtxn name=mytxn` | `searchtxn startswith="login" endswith="logout"` | `searchtxn maxspan=1h` | `searchtxn maxevents=50` |
| selfjoin | `selfjoin user` | `selfjoin session_id` | `selfjoin host max=2` | `selfjoin user keepevents=true` |
| sendalert | `sendalert my_alert` | `sendalert my_alert param.to="user@example.com"` | `sendalert my_alert param.subject="Alert"` | `sendalert my_alert action.email=true` |
| sendemail | `sendemail to="user@example.com"` | `sendemail to="user@example.com" subject="Report"` | `sendemail to="user@example.com" format=table` | `sendemail to="user@example.com" sendpdf=true` |
| set | `set diff [ search index=a ] [ search index=b ]` | `set intersect [ search index=a ] [ search index=b ]` | `set union [ search index=a ] [ search index=b ]` | `set diff [ savedsearch=a ] [ savedsearch=b ]` |
| setfields | `setfields app="web"` | `setfields env="prod"` | `setfields role="admin"` | `setfields app="web" env="prod"` |
| sichart | `sichart count BY sourcetype` | `sichart avg(bytes) BY host` | `sichart count BY host status` | `sichart sum(bytes) BY uri` |
| sirare | `sirare host` | `sirare uri` | `sirare 10 user` | `sirare limit=20 showcount=true dest_ip` |
| sistats | `sistats count BY sourcetype` | `sistats sum(bytes) BY host` | `sistats avg(latency) BY uri` | `sistats dc(user) BY src_ip` |
| sitimechart | `sitimechart count BY sourcetype` | `sitimechart sum(bytes) BY host` | `sitimechart avg(latency) BY uri` | `sitimechart dc(user) BY src_ip` |
| sitop | `sitop host` | `sitop 20 uri` | `sitop 10 user BY host` | `sitop limit=5 src_ip` |
| sort | `sort _time` | `sort -_time` | `sort host _time` | `sort 0 -_time` |
| spath | `spath` | `spath output=payload path=data.payload` | `spath input=_raw` | `spath path="root.items{}"` |
| stats | `stats count` | `stats count BY sourcetype` | `stats avg(bytes) BY host` | `stats sum(bytes) BY host status` |
| strcat | `strcat host ":" port " " endpoint AS dest` | `strcat user "@" domain AS email` | `strcat method " " uri AS request` | `strcat src_ip ":" src_port AS src` |
| streamstats | `streamstats count` | `streamstats sum(bytes) AS running_bytes` | `streamstats dc(user) AS users BY host` | `streamstats avg(latency) AS avg_lat BY host` |
| table | `table _time host sourcetype` | `table host user status` | `table src_ip dest_ip bytes` | `table _time host uri status bytes` |
| tags | `tags host` | `tags sourcetype` | `tags host=appserver` | `tags sourcetype=access_combined` |
| tail | `tail 10` | `tail 5` | `tail 100` | `tail 1` |
| timechart | `timechart count BY sourcetype` | `timechart sum(bytes) BY host` | `timechart avg(latency) span=5m BY uri` | `timechart dc(user) span=1h BY src_ip` |
| timewrap | `timewrap 1d` | `timewrap 1w` | `timewrap 1h series=relative` | `timewrap 1d align=time` |
| tojson | `tojson` | `tojson indent=2` | `tojson outputfield=json` | `tojson pretty=t` |
| top | `top host` | `top 20 uri` | `top status BY host` | `top limit=5 user BY src_ip` |
| transaction | `transaction session_id` | `transaction startswith="login" endswith="logout"` | `transaction maxspan=1h` | `transaction maxevents=50 keepevicted=t` |
| transpose | `transpose` | `transpose 5` | `transpose column_name=metric` | `transpose 0 header_field=metric` |
| trendline | `trendline sma5(count)` | `trendline ema10(bytes)` | `trendline sma3(avg_bytes)` | `trendline wma5(count)` |
| tscollect | `tscollect` | `tscollect index=summary` | `tscollect marker="daily"` | `tscollect maxspan=1h` |
| tstats | `| tstats count WHERE index=_internal BY sourcetype` | `| tstats sum(bytes) WHERE index=main BY host` | `| tstats avg(latency) WHERE index=web span=5m BY uri` | `| tstats dc(user) WHERE index=auth BY src_ip` |
| typeahead | `| typeahead prefix="sea"` | `| typeahead prefix="ind"` | `| typeahead prefix="erro"` | `| typeahead prefix="stat"` |
| typelearner | `typelearner` | `typelearner learn=true` | `typelearner maxtypes=50` | `typelearner maxterms=100` |
| typer | `typer` | `typer maxterms=50` | `typer maxtypes=20` | `typer field=eventtype` |
| union | `union maxtimes=2` | `union max=0` | `union keepempty=true` | `union maxsearches=10` |
| uniq | `uniq` | `uniq field=host` | `uniq start=1` | `uniq field=user` |
| untable | `untable _time metric value` | `untable host metric value` | `untable _time field value` | `untable metric field value` |
| walklex | `| walklex index=_internal` | `| walklex index=main` | `| walklex index=*` | `| walklex index=security` |
| where | `where status=500` | `where bytes>100000` | `where like(uri,"/api/%")` | `where in(status,(400,404,500))` |
| x11 | `x11 field=value` | `x11 field=value mode=additive` | `x11 field=value mode=multiplicative` | `x11 field=value ta=7` |
| xmlkv | `xmlkv` | `xmlkv maxattrs=10` | `xmlkv field=payload` | `xmlkv recursive=true` |
| xmlunescape | `xmlunescape field=_raw` | `xmlunescape field=payload` | `xmlunescape` | `xmlunescape field=message` |
| xpath | `xpath outfield=fieldname "//tag/text()"` | `xpath field=_raw outfield=ip "//ip/text()"` | `xpath outfield=value "//value/text()"` | `xpath field=payload outfield=code "//code/text()"` |
| xyseries | `xyseries _time host bytes` | `xyseries host metric value` | `xyseries _time uri latency` | `xyseries src_ip dest_ip count` |
