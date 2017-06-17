---
title: Dadgum Box Scores | Officials
layout: refs
---

# Dadgum Box Scores 

## Officials game-by-game 2016-17

#### Filter by a referee's first or last name


<pre class="huffman stilwata">
Most Frequent Officials
|      Name     |  # of Games |
|:-------------:|:-----------:|
 |   Ron Groover |      8      | 
|  Mike Eades   |      7      |
| Ted Valentine |      6      |
</pre>


<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th class="nate">Location</th>
           <th class="britt">Rating</th>
           <th class="larrydrew nate" data-sortable="false">Ref 1</th>
           <th class="larrydrew nate" data-sortable="false">Ref 2</th>
           <th class="larrydrew nate" data-sortable="false">Ref 3</th>
           <th class="janet" data-sortable="false">Box Score</th>
         </tr>
     </thead>

    <tbody>
	{% for off in site.data.offs %}
		<tr>
  			<td class="nate">{{ off.location }}</td> 
        <td class="britt">{{ off.rtg }}</td> 
        <td class="larrydrew nate">{{ off.off1 }}</td> 
  			<td class="larrydrew nate">{{ off.off2 }}</td>
  			<td class="larrydrew nate">{{ off.off3 }}</td>
        <td class="janet"><span style="background-color:#{{ off.style }}; padding: 2px 2px;"><a href="{{ off.box }}" target="_blank">{{ off.game }}</a></span></td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


