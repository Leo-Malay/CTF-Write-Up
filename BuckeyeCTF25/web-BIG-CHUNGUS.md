# BIG CHUNGUS

**Tags:** web

**Link:** [https://big-chungus.challs.pwnoh.io/](https://big-chungus.challs.pwnoh.io/)

**Problem Statement:** There's wabbit twouble afoot! `https://big-chungus.challs.pwnoh.io/`

**Solution:** After visiting the website and trying different input, I quickly realized that the form is making a get request with `username` in the query field. Then I downloaded the source code where I found the problematic condition `if (req.query.username.length > 0xB16_C4A6A5) {}`. Now only If I am somehow able to bypass it, I will get the flag. Thus what if I pass something like username: {length: "SOME_THING_BIGGG"}... well it should work and it did!! Thus after some digging, I figured the way for sending the JSON -> `username[length]=5000000000000000000000`
