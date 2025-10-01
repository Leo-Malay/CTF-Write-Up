# SQL Inject

**Problem Statement:** No fun flavortext. Just a SQL Injection challenge. (SQL is actually so cool and awesome but I couldn't think of ANYTHING fun to do with this one)

**URL:** [https://sql.watthewat.me/](https://sql.watthewat.me/)

**Approach:** I tried inserting the some common names to see how it reall works. Then I moved to source code inspection. I observed that it is making a GET reauest to the server. So, I tried inserting the most basic query and it worked.

**Solution:** `' OR 1=1; --`

![Original]("/webpage.png")
![Proof]("/proof.png")
