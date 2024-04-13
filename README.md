![alt text](https://i.imgur.com/reZZPp3.png {width=60px height=60px})

[center][size=25]**Tavtie Design**[/size][/center]

![](https://i.imgur.com/DFZbQvx.png | width=368) ![](https://i.imgur.com/S0Wpm3n.png | width=368)
![](https://i.imgur.com/8HlHnzi.png | width=368)

### About The Design
This design is inspired by the Asirem theme. I reached this design by making a few changes on the default theme of Flarum. I want to share it with you, thinking you will like it.

The parts I edited;
- I made the dropdown menus with a smoother design.
- I adapted the Afrux widget plugin to this design.
- I organized the discussion page.
- I edited the profile page.
- I removed the sidebar of the blog page, so it became a full blog page.
- I organized the design of the tags page.
- If you add a poll to your discussion, you can see that it has also been edited.
- I added a customized scroll bar.
- I softened the corners of iframe plugins.

### Installation
All you need to do is copy and paste the following css code into the Custom Css section on the admin/appearance page.

```
/* THEMES ########################################################### */
:root {
    --border-radius: 14px !important;
    --discussion-title-color: #636d79;
}

.Dropdown-menu {
    padding: 8px;
}

.Dropdown-menu>li>a, .Dropdown-menu>li>button, .Dropdown-menu>li>span {
    border-radius: var(--border-radius);
}

.AfruxWidgets-Widget-content {
    border-radius: var(--border-radius) !important;
}

.AfruxWidgets-Widget-title {
    font-weight: 600;
}

.DiscussionListItem-title {
    font-weight: 600;
}
/* ####################### HERO ########################### */
.Hero {
    z-index: 0;
    max-width: 1200px;
    margin: 15px auto 0px;
    border-radius: var(--border-radius);
}

@media (min-width: 1100px) {
.Hero {
    width: 1100px;
}}

@media (min-width: 992px) and (max-width: 1099.98px) {
.Hero {
    width: 992px;
}}

@media (min-width: 768px) and (max-width: 991.98px) {
.Hero {
    width: 768px;
}}

@media (max-width: 767.98px) {
.Hero {
    max-width: 97%;
    margin-bottom: 15px;
}}

.DiscussionHero .TagsLabel .TagLabel {
    border-radius: 14px !important;
}

/* ####################### HERO END ####################### */
/* ####################### PROFİLE ######################### */

.UserHero, .CoverEditor-cover, body.dark .UserPage .Hero, .UserCard {
    background-size: cover !important;
    border-radius: var(--border-radius);
}

.darkenBackground {
    border-radius: var(--border-radius);
}

.social-settings>.fa-cog {
    border-left: 1px solid transparent !important;
    width: 120%;
    margin-left: 5px;
}

.UserBadge {
    border-radius: var(--border-radius) !important;
    font-weight: 500;
}

.PostsUserPage-list>li {
    border-bottom: 2px solid var(--control-bg);
    background: #3464870a;
    border-radius: 14px;
    padding: 15px;
}

.LinkedAccounts-Account {
    border-radius: var(--border-radius) !important;
}

.trumbowyg-button-pane {
    border-radius: var(--border-radius) var(--border-radius) 0 0;
}

.trumbowyg-box, .trumbowyg-editor {
    border-radius: var(--border-radius);
}

/* Menu Font Bold */
.LinksButton-title {
    font-weight:bold;
}

.Dropdown-menu>li>a, .Dropdown-menu>li>button, .Dropdown-menu>li>span {
    font-size: 14px;
}

.SocialButtonsModal .Modal-content {
    overflow: auto !important;
}

.UserCardBadgesModal .UserCardBadgesModalCategory-badge {
    border-radius: var(--border-radius) !important;
}

.UserBio {
    border-radius: var(--border-radius) !important;
}

.UserDirectoryList .UserCard--directory, .UserDirectoryList .UserCard--directory .darkenBackground {
    border-radius: var(--border-radius) !important;
}

.item-fofsocialprofile {
    background: #ffffff33;
    border-radius: var(--border-radius);
    padding: 0px 3px;
}

.UserBirthdaysList-users li {
    border-radius: var(--border-radius) !important;
}

.UserBirthdaysList-main .UserStats {
    font-weight: 500;
}

/* ####################### TAGS PAGE ############################# */

.TagTiles {
    display: grid;
    grid-template-columns: repeat(2, 48%);
    list-style: none;
    gap: 8px;
}

@media (min-width: 992px) {
.TagTiles>li {
    float: left;
    width: 100% !important;
}}

@media (min-width: 768px) and (max-width: 991.98px) {
.TagTiles>li {
    float: left;
    width: 100% !important;
}}

@media (max-width: 767.98px) {
.TagTiles {
    grid-template-columns: 100% !important;
    padding: 10px !important;
}}

.TagsPage .container {
    max-width: 97% !important;
}

.TagTiles>li {
    border-radius: var(--border-radius) !important;
}

/* ####################### POLL ################################# */
.PollOption .PollOption-active {
    background-color: var(--primary-color) !important;
}

.PollOption .PollBar {
    border-radius: var(--border-radius) !important;
    border: 2px solid #191e2526 !important;
}

.Post-poll {
    border-radius: var(--border-radius);
    background: #2d466f17;
    padding: 10px;
}

/* ####################### COMMENT ################################# */
.ReplyPlaceholder:hover {
    border-color: var(--control-bg);
    border: 2px solid var(--control-bg);
    border-radius: var(--border-radius) !important;
}

/* ####################### OTHER ################################# */
@media (max-width: 767.98px){
.PostStream-item:not(:last-child) {
    margin: 20px 5px 10px 5px !important;
    padding: 0 15px;
}}

@media (max-width: 767.98px) {
.open.Dropdown .Dropdown-menu {
    border-radius: 14px;
    padding: 8px;
    margin: 8px;
}}

.MobileTab {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 97% !important;
    background: #fff;
    box-shadow: 0 2px 6px rgba(0,0,0,0.35);
    z-index: 1000;
    margin: 8px;
    border-radius: var(--border-radius);
}

@media (max-width: 767.98px) {
.DiscussionListItem-title {
    font-size: 15px !important;
    text-decoration: none !important;
}}

.DiscussionListItem-info {
    font-size: 12px;
}

/*Scroll*/
::-webkit-scrollbar {
    width: 6px;
    height: 6px;
}
::-webkit-scrollbar-button {
    display: none;
}
::-webkit-scrollbar-thumb {
    background: var(--primary-color);
    min-height: 5rem;
    border-radius: 1rem;
    border-left: 4px solid var(--trow-bg);
    border-right: 4px solid var(--trow-bg);
}

.Header-controls .item-signUp {
    display:none !important;
}

@media (max-width: 767.98px) {
.item-discussion-views {
    position: absolute;
    right: 80px;
}}

/* iframe köşe yumuşatma*/
.Post-body iframe {
    max-width: 100%;
    border-radius: 15px;
}

/* spoiler köşe yumuşatma */
span.spoiler {
    background: #444;
    color: transparent;
    border-radius: 5px;
}

/*Blog Hide Sidebar*/
.FlarumBlog-Article-Sidebar{
    display:none;
}
.FlarumBlog-Article-Container{
    margin-right:0 !important;
}
.FlarumBlogOverview .BlogFeatured-list-item-details h4 {
    font-weight:bold !important;
}

/* BLOG PAGE ################ */
.BlogSideWidget {
    border-radius:14px !important;
}
.FlarumBlogOverview .BlogScrubber .BlogList-item {
    border-radius:14px !important;
}
.FlarumBlogOverview .BlogScrubber .BlogList-item-photo {
    border-radius: 14px 0 0 14px;
}
.FlarumBlogOverview .BlogFeatured-list-item {
    border-radius:14px !important;
}
.FlarumBlogOverview .BlogFeatured-list-item-top .dataItem {
    border-radius:14px !important;
}
.FlarumBlogItem .FlarumBlog-Article .FlarumBlog-Article-Container .FlarumBlog-Article-Post .Post {
    padding:35px !important;
}
.FlarumBlogItem .FlarumBlog-Article .FlarumBlog-Article-Container .FlarumBlog-Article-Image {
    border-radius: 14px 14px 0 0;
}
.FlarumBlogItem .FlarumBlog-Article .FlarumBlog-Article-Container .FlarumBlog-Article-Content {
    border-radius: 14px;
}
@media (max-width: 767.98px) {
.BlogForumNav {
    display:none;
}}
/* THEMES END ####################################################### */
```

### Links
- [Github](https://github.com/stasarr)
- [Demo Link](https://forum.staup.online)
