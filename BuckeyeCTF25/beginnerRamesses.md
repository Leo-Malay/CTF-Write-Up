# Beginner/Ramesses

**Tags:** web

**Link:** [https://ramesses.challs.pwnoh.io](https://ramesses.challs.pwnoh.io)

**Problem Statement:** This is a good web challenge to start with. Use the help button to ask for a hint if you get stuck. Do you dare enter the tomb of Pharaoh Dave Ramesses? `https://ramesses.challs.pwnoh.io`

**Solution:** 

1. Inspected the website and found that session key is used. 
2. Downloaded the code and then found out that session key is nothing but Base64 encoded string with a flag `is_pharoh: false`, I decoded it, switched the boolean to true and encoded it. 
3. I was then able to access the flag.
