---
title: Dadgum Box Scores | Officials
layout: factors
---

# Dadgum Box Scores 

## NBA Draftees 2005-2016


<p class="huffman stilwata ford">Players shown if selected in NBA draft or if played in an NBA game. Data and <b>estimated on court earnings</b> are pulled from <a href="http://www.spotrac.com/nba/rankings/">Sportrac</a> and <a href="http://www.basketball-reference.com/" >Basketball-Reference</a>.</p> 

<p class="huffman stilwata ford">If you spot an error or have a suggestion, please send me an <a href="mailto:cbbstatshelp@gmail.com" >email here</a>.</p>

<br>

<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th class="larrydrew nate" >Player</th>
           <th class="larrydrew nate" >Class</th>
           <th class="larrydrew nate" >Drafted Team</th>
           <th class="janet">Year</th>
           <th class="janet">Pick #</th>
           <th class="larrydrew janet" >Games Played</th>
           <th class="larrydrew janet" >~On court Earnings</th>
         </tr>
     </thead>

    <tbody>
	{% for thenba in site.data.thenbas %}
		<tr>
        <td class="larrydrew nate">{{ thenba.player }}</td> 
        <td class="larrydrew nate">{{ thenba.classyear }}</td>
        <td class="larrydrew nate">{{ thenba.draftedteam }}</td>
  			<td class="janet">{{ thenba.theyear }}</td> 
        <td class="janet">{{ thenba.thepicknumber }}</td> 
        <td class="larrydrew janet">{{ thenba.gamesplayed }}</td>
        <td class="larrydrew janet">{{ thenba.careersalary }}</td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


