```javascript
string sCallBack = @"
    Sys.Application.add_load( 
       function() { if ( parent.document.getElementById('frame1') != null ) {               
                             $find('mpLoad').show(); XXX } else { $find('mpLoad').show(); XXX }
                  } 
    ); 
ScriptManager.RegisterStartupScript(this, this.GetType(), "alertSaveOk", sCallBack, true);
