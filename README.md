# Data-statistics
Data statistics
$.ajax({

  url: "/feeds/posts/default?alt=json-in-script",

  type: "get",

  dataType: "jsonp",

  success: function(data) {

    var totalposts = data.feed.openSearch$totalResults.$t;

    $('.total-posts').html(totalposts);

  }

});
