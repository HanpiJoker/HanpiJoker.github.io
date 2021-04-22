---
layout: post
author: "HanpiJoker"
title: "Vim 指令学习"
---

## Vim Command
> Learning from youtube video: [vim + tmux](https://www.youtube.com/watch?v=5r6yzFEXajQ)

Ubuntu: *sudo apt-get install vim  
CentOS: *sudo yum install vim*  
...  
(ps: This is so easy!)

### 1. Modal Editing

**Normal Mode** -- navigate(导航) the structure of the file  
**Insert Mode** -- editing the file  
**Visual Mode** -- highlight portions of the file to manipulate(操作) at once  
**Ex Mode**     -- command mode  

**DON'T USE ARROW KEYS**  
**DON'T USE THE MOUSE**  

### 2. h j k l (Move Fast)
h -- left  
j -- down  
k -- up  
l -- right  

*[ps: ^E means Ctrl-E， scroll(滚动)，cursor(光标)]*  
^E -- scroll the window down  
^Y -- scroll the window up  
^F -- scroll down one page  
^B -- scroll up one page  
H  -- move cursor to the top of the window  
M  -- move cursor to the middle of the window  
L  -- move cursor to the bottom of the window  
gg -- go to top of file  
G  -- go to bottom of file  

### 3. The secret sauce
> text objects and motions  
> the DOT command  
> macros (宏)  

#### Text Objects And Motions

text objects

    w -- words
    s -- sentences
    p -- paragraphs
    t -- tags 

motions

    a -- all
    i -- in
    t -- til
    f -- find forward
    F -- find backward

Commands

    d -- delete (also cut)
    c -- change (delete, then place in insert mode)
    y -- yank (copu)
    v -- visually select

**{command}{text object or motion}**
> eg:
>   1. diw (delete in word)
>   2. caw (change all word)
>   3. yi) (yank all text inside parentheses)
>   4. dt< Space >  (delete until space)
>   5. df< Space >  (delete including space)
>   6. va" (visually select all inside doublequotes including doublequotes)


#### Repetition The DOT(.) command
**.** &#160; ：Repetition the last command

#### Additional Commands
dd/yy -- delete/yank the current line  
D/C   -- delete/change until end of line  
^/$   -- move to the beginning/end of line  
I/A   -- move to the beginning/end of line and insert  
O/o   -- insert new line above/below current line and insert  

( ps: :earlier 2m means go to the file two minutes ago )  

**Try and make actions repeatable**  
**Practice it**  

#### Macro
*A sequence of commands recorder to a register*
1. Record a macro
> q{register}
> (do the things)
> q
2. Play a macro
> @{register}

3. press m-key to set a tag named key, then you can press "tilde-key" to go back)  
[tilde means '~']

4. :reg  
> You can use :reg to open you register lists, and you can find what things 
> in the registers。you can also use "< num > to choose the register, and then  
> you can use "< num >p to paste the words in the regiseter 

**It's so interesting!!** 

