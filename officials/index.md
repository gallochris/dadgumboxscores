---
title: Dadgum Box Scores | Officials
layout: refs
---

# Dadgum Box Scores 

## Officials game-by-game 2016-17

#### Last updated: 2-22-2017

#### Filter by a referee's first or last name

#### Crew composite rating is pulled using [Ken Pomeroy's data](http://kenpom.com/officials.php). 


<pre style="text-align: center">
Most Frequent Officials
|      Name     |  # of Games |
|:-------------:|:-----------:|
| Ted Valentine |      5      |
|  Roger Ayers  |      5      |
|  Ron Groover  |      5      |
</pre>

<pre style="text-align: center">
Best Crew Rating
|      Game     | Rtg Total|
|:-------------:|:--------:|
| Virginia Tech |     23   |
|      Duke     |     23   |
|   Lousiville  |     35   |
</pre>


<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th data-sortable="false">Box Score</th>
           <th class="larrydrew">Location ↑↓</th>
           <th class="larrydrew">Rating ↑↓</th>
           <th data-sortable="false">Ref 1</th>
           <th data-sortable="false">Ref 2</th>
           <th data-sortable="false">Ref 3</th>
         </tr>
     </thead>

    <tbody>
	{% for ref in site.data.refs %}
		<tr style="background-color: #{{ ref.style }};">
  			<td><a href="{{ ref.box }}" target="_blank">{{ ref.game }}</a></td>
  			<td class="larrydrew">{{ ref.location }}</td> 
        <td class="larrydrew">{{ ref.rtg }}</td> 
        <td>{{ ref.off1 }}</td> 
  			<td>{{ ref.off2 }}</td>
  			<td>{{ ref.off3 }}</td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


