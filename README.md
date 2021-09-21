# General

Create ServerInfo With UI

# Commands

Commands | Default
--- | ---
`/serverinfo` | True

# Feature
- You can Create, Your custom subcategory
- Add Button On subcategory
- Set Action For Button
- Set Title For subcategory
- Set Content For subcategory
- Send subcategory for First Player Join
- Send subcategory For Player Join

# ToDo List
- Per subcategory have permissions
- Per Button have permissions
- Edit subcategory In Game

I don't know if I will do it or not, because I'm lazy hahaha :)

# Config

``` YAML

---
# Send Info 
# On First Player Join
on-first-join: true
# subcategory Form
join-first-form: "rules"

# Send Info
# On Player Join
on-join: true
# subcategory Form
join-form: "welcome"

# All subcategoryform
# Tag Form
# {NAME} Name The Player
# {DISPLAY_NAME} Display Name The Player
subcategory-form:
 rules:
  title: "Rules"
  content:
   - "Hi {NAME}, Please Read Rules Below"
   - "- In This Server Don't Grief"
   - "- Don't Abuse"
   - "- Don't Spam Chat"
   - ""
   - "If You Accepted The Rules"
   - "Press The Button Below:"
  button:
   0:
    text: "YES"
    action:
     - "msg {NAME} Thx For Accepting"
   1:
     text: "NO"
     action:
      - "kick {NAME} Accept Rules Please"
 welcome:
  title: "Welcome"
  content:
   - "Hi {NAME}, Thx For Joining"
   - "Please Accept The Rules"
   - "if you haven't read it"
  button:
   0:
    text: "PLAY"
    action:
     - "msg {NAME} Have a nice play"
   1:
     text: "READ RULES"
     action:
      - "rca {NAME} serverinfo rules"
...
```

# Additional Notes

- If you find bugs or want to give suggestions, please visit [here](https://github.com/MulqiGaming64/ServerInfo/issues)
- Icons By [icons8.com](https://icons8.com)
