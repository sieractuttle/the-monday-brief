STRATEGY FIELD NOTES — how this site works
=============================================

FOLDER STRUCTURE
  index.html          the homepage, lists every week
  style.css            shared design, used by every page
  weeks/week-01.html   week 1, already written
  weeks/template.html  copy this to add a new week

ADDING A NEW WEEK
  1. Copy weeks/template.html and rename it, e.g. weeks/week-02.html
  2. Replace everything in [BRACKETS] with that week's content
  3. Duplicate the <div class="card">...</div> block until you have 5,
     updating "01 / 05" through "05 / 05"
  4. Open index.html, copy the <a class="week-row">...</a> block for
     Week 01, update the link, week number, title, and one-line summary,
     and paste it above the "Week 02 goes here" placeholder row
  5. Save. That's it, no build step, no install.

  If it's easier, just send me next week's readings and I'll write the
  post and the tip cards and drop the files in for you.

SHARING WITH YOUR CLASS
  This is a static site (plain HTML files), so there's no server needed
  to build it, but you do need somewhere to host it for a shareable link.
  Two easy free options:

  A) Netlify Drop (fastest, no account required)
     1. Go to https://app.netlify.com/drop
     2. Drag the whole "strategy-field-notes" folder onto the page
     3. It gives you a live URL immediately, share that link

  B) GitHub Pages (free, more permanent, needs a free GitHub account)
     1. Create a new repository on github.com
     2. Upload all the files in this folder (keep the weeks/ subfolder)
     3. In the repo, go to Settings > Pages, set the source to the
        main branch, save
     4. GitHub gives you a URL like yourname.github.io/repo-name

  If your class uses Canvas, you can also just upload the whole folder
  as a zip file for classmates to download and open index.html locally,
  no hosting needed at all, though a link is easier to click from a post.

EDITING THE LOOK
  All the styling lives in style.css. Colors are set as variables at the
  very top of that file (--paper, --ink, --ochre, --teal, etc.) if you
  ever want to adjust the palette without touching individual pages.
