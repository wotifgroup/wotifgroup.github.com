---
layout: full
title: WotifGroup Architecture Radar - Apr 2011 
category: Architecture
tags:
  - architecture
  - radar
---

The WotifGroup Architecture Radar is "our" version of the <a href="http://www.thoughtworks.com/radar">ThoughtWorks Technology Radar</a>.

<script type="text/javascript" src="/js/radars/lib/protovis-3.2/protovis-d3.2.js"></script>

<script type="text/javascript" charset="utf-8" src="/js/radars/utils.js"></script>

<script type="text/javascript" charset="utf-8" src="/js/radars/radars/wotifgroup_tech_radar_feb_2011.js"></script>
 
<style type="text/css" media="screen">
  
#fig {
  height: 1000px;
  width: 1200px;
}
 
</style>

<div style="display:none">Don't display this field, but it is here to ensure the radar doesn't show up on the index pages in a page-width that is too small</div>
<script type="text/javascript" src="/js/radars/radar.js" charset="utf-8"></script>

<div id="radar" style="background-color='#000;'"></div> 

<script type="text/javascript">
 
var h = 1160;
var w = 1200;
 
$(document).ready(function() {radar_init(h,w); } );

</script>
