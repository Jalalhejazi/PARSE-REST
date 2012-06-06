
PARSE.com (The mobile app platform for developers)


Save flexible data objects to the cloud with SDKs for iOS, Android, JavaScript, and a REST API. No servers necessary.

JAVASCRIPT> 

var BlogPost = Parse.Object.extend("BlogPost");
var blogPost = new BlogPost();

blogPost.save({
  title: "Hello World"
}, {
  success: function(blogPost) {
    // The object was saved successfully.
  },
  error: function(blogPost, error) {
    // The save failed.
  }
});