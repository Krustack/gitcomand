  ## 🚩<span style="color: red;">git command เบื้องต้น</span>

💡`git init`  การสร้าง local repository

💡`git add <ชื่อไฟล์>`  การสร้าง การอัพไฟล์ขึ้นมาในstage

💡`git add .`  การสร้าง การอัพไฟล์ขึ้นมาในstageทั้งหมดที่มีการอัพเดท

💡`git commit -m "ชื่อcommit"`  การสร้าง การอัพไฟล์ขึ้นมาในstageทั้งหมดที่มีการอัพเดท

💡`git remote add origin <path>`  การโยงlocal repositoryกับremote repository

💡`git push -u origin <branch>`  การอัพcode ขึ้น remote ใช้ในครั้งแรก

💡`git push`  การอัพcode ขึ้น remote 

💡 `git pull`  นำcodeจาก remote มาใน local

 ## 🚩<span style="color: red;">git command ในการจัดการ branch</span>
 
 🚀 `git branch`  ใช้ดู branch ที่มีทั้งหมด
 
 🚀 `git branch <ชื่อ>`  ใช้สร้าง branch
 
 🚀 `git checkout <ชื่อ>`  ใช้เปลี่ยน branch ทำงาน
 
 🚀 `git branch -d <ชื่อ>`  ลบbranch
 
 🚀 `git branch -D <ชื่อ>` ลบbranch ในกรณีที่ไม่ได้merge branch กับbranch อื่น
 
  ## 🚩<span style="color: red;">git command ดูข้อมูล</span
  
  🔎 `git status`	ดูสถานะการเปลี่ยนแปลงใน local repository
  
  🔎 `git log`	ดูข้อมูลการ commitของเรา
  
  🔎 `git log -- oneline`	ดูข้อมูลการcommitของเราแบบย่อ
  
  🔎 `git diff <hash>`	เทียบการเปลี่ยนแปลงในcommit ปัจจุบันกันตัวhash
  
  🔎 `git diff <hash> <hash>`	เทียบการเปลี่ยนแปลงในcommit hashกับhash
  
  ## 🚩<span style="color: red;">git command ลบข้อมูล</span
  
  🎃`git checkout HEAD <ชื่อไฟล์>`	ยกเลิกข้อมูลในไฟล์นั้นไปเป็น commit ล่าสุด
  
  🎃`git reset --hard HEAD`	ยกเลิกข้อมูลทุกไฟล์บนstageไปเป็น commit ล่าสุด
  
  🎃`git reset <hash>`	ย้อนข้อมูลไปยังcommit hash ที่เราเลือก จะมีการเก็บข้อมูลอื่นๆอยู่ใน stage
  
  🎃`git reset --hard <hash>`	ย้อนข้อมูลไปยังcommit hash ที่เราเลือก ไม่มีการเก็บข้อมูลอะไรไว้
  
  🎃`git revert <hash>`	นำcode ในhashมาอัพเดทใช้ในcommit ปัจจุบัน
