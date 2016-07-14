===== README =====

 This is a blog application created for exercise and learning purposes. <br>
 Ruby version is- ruby 2.3.0p0 (2015-12-25 revision 53290)<br>
I used Cloud9, GitHub and BitBucket to create this application<br>
 <h3>In C9, Create a new Blank workspace <h3/> <br>
 In command prompt-<br>
 <tt>gem install rails </tt>   (to see version- $ <tt>rails -v </tt>,  $<tt> ruby -v </tt>)<br>
<tt>rails new blog </tt>      (this creates a new folder with rails application)<br>
Initialize empty Git repository - $ <tt>git init</tt><br>
Create a new repository (GitHub & BitBucket)<br>
Check to see if all remote repositories connected - $ <tt>git remote -v show</tt><br>
Change Read Me file<br>

<h3>Heroku-<h3/> (since I already have a heroku account)<br>
<tt>which heroku</tt> (check if heroku is installed in C9)<br>
<tt>heroku login </tt>(login to heroku account from C9)<br>
<tt>heroku create vish-blog </tt>- (This creates a "vish-blog” app in heroku)<br>

<h3>Push the code-<h3/><br>
Change gem file before pushing to heroku – remove gem 'sqlite3' and add- 
<tt>group :development, :test do
    gem 'byebug'
    gem 'sqlite3'</tt>
<tt>group :production do
    gem 'pg'</tt>
Add all files - $<tt> git add .</tt>   OR <tt>git add -A</tt><br>
<tt>git commit -m "First commit"</tt><br>
<tt>git push</tt><br>

<tt>git push heroku master</tt><br>
Run rails server - $ <tt>rails server -b $IP -p $PORT</tt><br>
