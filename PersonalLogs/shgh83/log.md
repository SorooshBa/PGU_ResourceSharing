git clone https://github.com/shgh83/PGU_ResourceSharing.git
cd PGU_ResourceSharing
cd PersonalLogs
mkdir shgh83
cd shgh83
echo "" > log.md
cd ..
cd ..
git add .
git commit -m "created log.md and added my username to contributors.md"
cd Courses
mkdir "Information Retrieval"
git add resources.md 
git add Courses/"Information Retrieval"/resources.md
git add PersonalLogs/shgh83/log.md
git commit -m "added resources.md and added the resources to it. changed the log.md"
git add Courses/"Information Retrieval"/resources.md
git commit -m "added more resources to my file"
git add Courses/"Information Retrieval"/resources.md
git commit -m "added youtube videos  to my file"
git add PersonalLogs/shgh83/log.md
git commit -m "added my last commands to log.md"
deleted the unwanted files that i commited accidentally