---
title: Dadgum Box Scores
layout: default
---

# Dadgum Box Scores 

## Every UNC Box Score Since 03-04

#### [Find the referees for each game](/officials/)

#### [16-17 game-by-game four factors breakdown](/four-factors/)

#### Filter by season, wins, losses, opponent or type of game

<table id="example" class="display center" cellspacing="0" width="100%" table-layout="fixed">
	<thead>
         <tr> 
          <th class="larrydrew nate">Type</th>
          <th class="larrydrew nate">Location</th>
          <th class="janet britt">Year</th>
          <th class="janet">Date</th>
          <th class="janet" data-sortable="false">Box Score</th>
          <th class="janet britt">Result</th>
         </tr>
     </thead>

    <tbody>
	{% for all in site.data.alls %}
		<tr>
        <td class="larrydrew nate">{{ all.type }}</td>
        <td class="larrydrew nate">{{ all.location }}</td>
        <td class="janet britt">{{ all.season }}</td> 
        <td class="janet">{{ all.date }}</td> 
        <td class="janet"><span style="background-color:#{{ all.style }}; padding: 2px 2px;"><a href="{{ all.box }}" target="_blank">{{ all.game }}</a></span></td>
        <td class="britt">{{ all.result }}</td>
                </tr>
  			{% endfor %}
    </tbody>
</table>


