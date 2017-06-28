---
title: Dadgum Box Scores | Officials
layout: refs
---

# Dadgum Box Scores 

## Officials game-by-game since 03-04 

#### Filter by a referee's name, result, location, season, or type of game


<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th class="britt">Location</th>
           <th class="britt">Type</th>
           <th class="boone nate" data-sortable="false">Ref 1</th>
           <th class="boone nate" data-sortable="false">Ref 2</th>
           <th class="boone nate" data-sortable="false">Ref 3</th>
           <th class="britt">Result</th>
           <th class="larrydrew janet">Season</th>
           <th class="boone janet" data-sortable="false">Box Score</th>
         </tr>
     </thead>

    <tbody>
	{% for off in site.data.offs %}
		<tr>
  			<td class="britt">{{ off.location }}</td> 
        <td class="britt">{{ off.type }}</td> 
        <td class="boone nate">{{ off.off1 }}</td> 
  			<td class="boone nate">{{ off.off2 }}</td>
  			<td class="boone nate">{{ off.off3 }}</td>
        <th class="britt">{{ off.result }}</th>
        <td class="larrydrew janet">{{ off.season }}</td>
        <td class="boone janet"><span style="background-color:#{{ off.style }}; padding: 2px 2px;"><a href="{{ off.box }}" target="_blank">{{ off.game }}</a></span></td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


