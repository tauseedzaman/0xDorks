# 0xDorks
## My collection of Awesome Google Dorks.

#### 🚧 **Staging & Beta**
> Discover open directories on beta or testing subdomains that may contain development files or overlooked data.
```dork
site:*beta.* "index of"
```


#### 🔐 **Login Pages**
```dork
inurl:login | inurl:adminlogin | intitle:"login page"
```
```dork
inurl:admin intitle:"admin login"
```

---

#### 📁 **Exposed Files**
```dork
intitle:"index of" "backup"
```
```dork
intitle:"index of" (mp3|pdf|doc|sql|zip)
```
```dork
inurl:"/phpinfo.php"
```

---

#### 🛑 **Sensitive Info Leaks**
```dork
filetype:env "DB_PASSWORD"
```
```dork
filetype:sql "INSERT INTO"
```
```dork
filetype:log password | email
```
```dork
intext:"AWS_ACCESS_KEY_ID" | "AWS_SECRET_ACCESS_KEY"
```

---

#### 📄 **Configuration Files**
```dork
intitle:"index of" ".git"
```
```dork
filetype:xml site:* ext:xml
```
```dork
filetype:json "auth" OR "credentials"
```

---

#### 🧠 **Tech Stack Info**
```dork
intitle:"phpinfo()" "PHP Version"
```
```dork
inurl:"/server-status" "Apache Status"
```

---

#### 🎯 **Open Directories**
```dork
intitle:"index of" site:*.gov
```
```dork
intitle:"index of" "parent directory"
```

---

#### 💀 **Security Cam / Webcams**
```dork
inurl:/view.shtml
```
```dork
intitle:"webcamXP 5"
```

---

### 🧪 Experimental / Unique Ideas
- Look for misconfigured Firebase DBs:
  ```dork
  site:.firebaseio.com inurl:.json
  ```
- Public Trello boards:
  ```dork
  site:trello.com inurl:boards
  ```
- GitHub dorks for secrets:
  ```dork
  site:github.com "SECRET_KEY"
  ```

---
