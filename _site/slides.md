template: title

.mega-octicon.octicon-mark-github[]

# Undo, Redo
# Change History
# with Git

---

template: section

.mega-octicon.octicon-mark-github[]

## Joshua Wehner

* **`@jaw6`**
* `jaw6@github.com`
* Minneapolis, MN, USA
* GitHub Training

---

template: content

# Undo & Redo
## Scenarios

http://bit.ly/some-url-here

---

template: body

# Undo "Public" Change .octicon.octicon-mark-github[]

* It's broken
* But it's pushed

```sh
git revert <sha>
```

---

template: body

# Tweak Last Commit .octicon.octicon-mark-github[]

* Oooops
* Committed too fast

```sh
git commit --amend
```

---

template: body

# Regrets, I've Had a Few .octicon.octicon-mark-github[]

* Ooooops
* That's mostly rubbish

```sh
git reset <last good sha>
```

---

template: body

# Throw It All Away .octicon.octicon-mark-github[]

* It's all rubbish
* I regret everything

```sh
git reset --hard <last good sha>
```

---

template: body

# Wait, On Second Thought .octicon.octicon-mark-github[]

* ~~Throw It All Away~~
* Could I maybe get that back?

```sh
git reflog
git reset --hard <sha>
```

---

template: body

# Well, That Wasn't So Bad .octicon.octicon-mark-github[]

* Most of that is trash
* But that one? That one is *good*.
* Gimme.

```sh
git cherry-pick <good one>
```

---

template: body

# Put That Thing Over There .octicon.octicon-mark-github[]

* I should have made this branch earlier
* Those commits should not be on `master`

```sh
git rebase master
```

---
name: image
background-color: #FFF
background-image: url(https://cloud.githubusercontent.com/assets/2077/5932295/2940c47a-a670-11e4-959e-dcc053c1082b.png)

--
name: image
background-color: #FFF
background-image: url(https://cloud.githubusercontent.com/assets/2077/5932294/293e17e8-a670-11e4-9f89-a13f5f83c135.png)

---

template: body

# Well, Then Again .octicon.octicon-mark-github[]

* Throw ~~It All~~ Some of It Away
* I regret that one thing
* Some of the rest of it was okay

```sh
git rebase -i <public sha>
```

---

template: body

# I Was Wrong Before .octicon.octicon-mark-github[]

* I thought I was wrong
* But I wasn't

```sh
git commit --fixup <sha>
git rebase -i --autosquash
```

---

template: body

# Forget I Said That .octicon.octicon-mark-github[]

* Stop tracking this file
* I mean it

```sh
git rm --cached
.gitignore
git clean -f`
(also `-x` maybe?)
```

---

template: section


.mega-octicon.octicon-mark-github[]

# Thank You!
## Undo, Redo, Change History
### **`@jaw6`**

http://training.github.com/
