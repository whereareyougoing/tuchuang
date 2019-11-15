# tuchuang
图床

需求

做基于evernote的个人知识库时，采用马克飞象爽了3天，evernote需要付费，然后10天，马克飞象就要付费，因此转成sublime结合evernote来做，图片必须采用外链的形式做，此时需要图床

PS：如果不需要发布，可以采用相对路径引用本地文件
其他工具

    七牛 可以考虑下，怕后期收费

以raw形式上传图片至github

请参照迁移博客图片者的福音：使用GitHub做免费不限流量图床

    1，在github创建repository

    2，利用github的windows客户端clone至本地

    3，将需要上传的文件放入本地的文件夹

    4，利用github的windows客户端commit

    5，网页浏览复制图片URL，如https://github.com/zhanghlHUST/figureForMarkdown/blob/master/17_urllib_parse_urlparse.JPG，将URL中blob替换为raw,即https://github.com/zhanghlHUST/figureForMarkdown/raw/master/17_urllib_parse_urlparse.JPG

延伸阅读

转载GitHubTricks: Upload Images & Live Demos
通过github的隐藏功能issue

当前Github上没有提供asset管理工具，但是利用Github中的issues特性可以进行CDN asset的管理，合理利用issues会使得上传文件到知识库特别简单，这些资料不会被commit/change跟踪，当在知识库中创建issues时，可以采用简单的drag-n-drop拖曳上传资源至repository, 步骤如下：

    1，创建一个新issue

18_issues_tab18_issues_tab

    然后拖曳图片进去，一次可以添加多个文件（然后发现直接图片的引用复制过来，粘贴到markdown）

19_upload_by_issue19_upload_by_issue

    上传完 issue 之后，就可以直接在图片上右键复制图片URL

