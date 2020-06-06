<script type="application/javascript">
    var tabs;
    var panels;
    var json;
     /*
    $.ajax({
        type:'GET',
        url:'https://whattheforum-sidebar-json.s3.amazonaws.com/sidebar.json',
        dataType:'json',
        async:true,
        success:function(data){
            json = data;
        }
    });
   
    $.getJSON( "https://whattheforum-sidebar-json.s3.amazonaws.com/sidebar.json", function( sidebarJson ) {
        json = sidebarJson; 
    }); */

  function generateArrays (parentstr) {
      parent = document.getElementById(parentstr);
      tabs = parent.querySelectorAll('[role="tab"]');
      panels = parent.querySelectorAll('[role="tabpanel"]');
      // Bind listeners
      for (i = 0; i < tabs.length; ++i) {
        addListeners(i);
      };
      loadSideBars(parentstr)
  };

 function loadSideBars(parentstr) {
    //alert(parentstr);
    
    $.ajax({
        type:'GET',
        url:'https://whattheforum-sidebar-json.s3.amazonaws.com/sidebar.json',
        dataType:'json',
        async:true,
        success:function(data){
            json = data;
            
            if(typeof json !== "undefined" ) {
                 if(typeof json[parentstr] !== "undefined") {
                    for (var i = 0; i < json[parentstr].length; i++){
                        populateSideBar(json[parentstr][i]['class'],json[parentstr][i]['source']);
                    }    
                 } else {
              }
            }
        }
    });

 }; 

  function addListeners (index) {

    tabs[index].addEventListener('click', clickEventListener);
    // Build an array with all tabs (<button>s) in it
    tabs[index].index = index;
  };

  // When a tab is clicked, activateTab is fired to activate it
  function clickEventListener (event) {

    var tab = event.target;
    activateTab(tab, false);
  };

  // Activates any given tab panel
  function activateTab (tab, setFocus) {
    parentNode = tab.parentElement.parentElement

    setFocus = setFocus || true;
    // Deactivate all other tabs
    deactivateTabs(parentNode);

    // Remove tabindex attribute
    tab.removeAttribute('tabindex');

    // Set the tab as selected
    tab.setAttribute('aria-selected', 'true');

    // Get the value of aria-controls (which is an ID)
    var controls = tab.getAttribute('aria-controls');

    // Remove hidden attribute from tab panel to make it visible
    document.getElementById(controls).removeAttribute('hidden');

    // Set focus when required
    if (setFocus) {
      tab.focus();
    };
  };

  // Deactivate all tabs and tab panels
  function deactivateTabs (parent) {
    tabs = parent.querySelectorAll('[role="tab"]');
    panels = parent.querySelectorAll('[role="tabpanel"]');

    for (t = 0; t < tabs.length; t++) {
      tabs[t].setAttribute('tabindex', '-1');
      tabs[t].setAttribute('aria-selected', 'false');
    };

    for (p = 0; p < panels.length; p++) {
      panels[p].setAttribute('hidden', 'hidden');
    };
  }
  
function populateSideBar(id,url) {
  var IdStr = '#'+id;
  var Id = $('#'+id);
  // first delete existing style class
  $('style.sidebar-class').remove();
  $.get(url, function(data){
    tableHtml = data.substring(data.indexOf('<table') + 6,data.indexOf('</table>'));
    tableHtml ='<table '+tableHtml+'</table>';
    tableHtml = tableHtml.replace(/\/\/images-docs-opensocial\.googleusercontent\.com\/gadgets\/proxy\?url=/g,'').replace(/.png&/g,'.png?');
    //console.log(tableHtml);
  
    styleHtml = data.substring(data.indexOf('.ritz'),data.indexOf('</style>')).replace(/.ritz .waffle/g,'');
    styleHtml = styleHtml.replace('.s0',IdStr+' .s0')
                .replace('.s1',IdStr+' .s1')
                .replace('.s2',IdStr+' .s2')
                .replace('.s3',IdStr+' .s3')
                .replace('.s4',IdStr+' .s4')
                .replace('.s5',IdStr+' .s5')
                .replace('.s6',IdStr+' .s6')
                .replace('.s7',IdStr+' .s7');

    styleHtml = '<style type="text/css" class="sidebar-class">'+styleHtml+' </style>';
    $('head').append(styleHtml);
    $(Id).html(tableHtml);
  });
}



</script>
