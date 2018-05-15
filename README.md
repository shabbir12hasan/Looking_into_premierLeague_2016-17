# Looking into premier league year 2016-17
##### (All graphs and images are stored in this folder: https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/tree/master/images)
Football is a beautiful game which is played aroud the word. And data analytics is one of most powerfull field these days. Both of these sentences aren't related too much however, if we combine both of them together as one then big meaning could be derived. "Data analytics in football", could deliver better insight and observations from different angles, it could be used to help a football team to learn more about its shortcoming while comparing them with other teams and by themselves.

#### What this report covers?
we have our data collected from this site: http://www.footballsquads.co.uk/archive.htm. Only premier league's data is collected during year 2016/17 for all 20 teams. We would look into these data sets and could try to understand different statistics of different teams.

Tasks
-  Data Wrangling: Cleaning data for all teams, removing unwanted variables and merging data of all players into one data frame.
-  Data Visualization: Analyzing patterns of data and understanding the data while visualizing it.

#### First lets have a look at teams for year 2016/17 are as follows:
Arsenal<br>
Bournemouth<br>
Burnley<br>
Chelsea<br>
Crystal Palace<br>
Everton<br>
Hull City<br>
Leicester City<br>
Liverpool<br>
Manchester City<br>
Manchester United<br>
Middlesbrough<br>
Southampton<br>
Stoke City<br>
Sunderland<br>
Swansea City<br>
Tottenham Hotspur<br>
Watford<br>
West Bromwich Albion<br>
West Ham United<br>


### Data Wrangling
Multiple data cleaning steps are involved in cleaning data once data is imported, and same data cleaning process will be applied on 20 other data sets of all teams.

Once we will clean data for all 20 teams then we will merge all records into one data frame and will perform operations on it.
Our data would look like this:
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/raw_team_data.PNG" width="450"/></p>

Now still we need to create few more variables which would help us to derive better results from our data, we would perform new operations in our whole data set of players.

#### New variables:
  - First rounding off value of height to 2 decimal places, and convert it into continous value.
  - Convert weight into continous value
  - Calculate BMI of players
  - Calculating age of players (While calculating age we would calculate age upto first matchday of premier league year 2016, basically that is 13-08-2016. Player's age would be calculated from their date of birth to this date.)
 
After changing and creating these variables, we would get clean data set and it would look like:
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/clean_team_data.PNG" width="450"/></p>

##### Data dictionary:
        - Name: Player's name
        - Nat: Nationality
        - Pos: preffered playing position
        - Height: player's height in meters
        - Weight: player's weight in kg
        - Date of Birth: Birth date
        - Current_Team: Team they are playing for
        - BMI: Body mass index of players
        - Age: player's age in years

### Data Visualization
Once we have our data cleaned, we can look into the data and find out what's happening in it. We will create visuals and elucidate it.
  1)  Which countries have most players playing in premier league?
  2)  Plotting height of players?
  3)  Plotting height and weight of players?
  4)  Comparing weight and age of players.
  5)  What does BMI index says?
  6)  Number of players in each teams?
  7)  Number of youth players in team(Unders 19).
  8)  Which month players are born?
    
  

## Lets Visualize.........

### 1)  Which countries have most players playing in premier league?
Lets plot a histogram for nationality of players,
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/players_nationality.png" width="950"/></p>

This graph shows that there are way lot of players from England, this as such really make sense. As, this is league from England. There would be lot of players from england. 

##### Now how about, we remove players with nationality as England, and then plot all the players.
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/international_players.png" width="950"/></p>

Changing angle of label as there were too many labels, which were making graph labels messy. Also, inserting colours for different countries to make data more clear.

With this graph it could be seen that apart from england, majority of players are from Spain, France and Ireland.

### 2)  Plotting height of players?
To identify players height, we can plot it through histogram.
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/players_height.png" width="950"/></p>

Plotting multiple graphs, different graph for different position. So, we can analyse what is the height variable in different position.
##### Position denote:
  - D : Defender
  - F : Forward
  - G : Goalkeeper
  - M : Midfielder
##### Form this graph it could be seen that relatively goalkeepers are tall and majority of defenders are also tall. Where as forwards are evenly splitted in height ranging from short to tall. And majority of midfielders are short heighted.


### 3)  Plotting height and weight of players?
We will plot height and weight of players according to their position, and then will analyse it.

<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/height_weight_comparision.png" width="950"/></p>

##### It could be seen that midfielders are short heighted and light weight, where as defenders and forwads have a smilar distribution.

### 4)  Comparing weight and age of players.
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/age_weight.png" width="950"/></p>

##### With this graph we could see that as age is increasing, players tend to gain more weight. Maybe this is because they gain more muscles over the period, or they gain more weigth as they are not able to keep up their fitness.

### 5)  What does BMI index says?
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/bmi.png" width="950"/></p>
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/bmi_meter.png" width="350"/></p>

##### Considering our finding we could see that majority of players have BMI around 22.5. When we check it into BMI meter it could be seen that average value is aound 20-25. However, we could see that few players have very high BMI, more than 25. What could be possible reasons? Although, atheltes usually have high BMI than normal people as they have more muscles in their body. But it could be possible that some of the players are out of shape and their fitness is not upto the marks.

### 6)  Number of players in each teams?
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/squad_strength.png" width="850"/></p>

### 7)  Number of youth players in team(Unders 19).
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/youth_squad.png" width="850"/></p>

Middlesbrough and West Ham had least number of youth players in their team. Where as Boremouth, Arsenal and Liverpool have lot of young players in their team.

### 8)  Which month players are born?
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/birth_month.png" width="950"/></p>

It could be seen that only few players share their birthdays during May, June and July month.
  
## Enough done for overall analysis abour players and positions, now we should look further into different teams.

### Visualizing teams....
  1) Average height of players in a team.
  2) Average weight of players in a team.
  3) Average age of players in a team.

### 1) Average height of players in a team.
<p align="center"><img src="https://github.com/shabbir12hasan/Looking_into_premierLeague_2016-17/blob/master/images/team_height_avg.png" width="850"/></p>

Clearly there is a big height difference between the team with tallest players and team with shortest players.
