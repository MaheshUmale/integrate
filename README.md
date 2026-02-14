# integrate
integration


INTEGRATE BACKEND and FROMNTEND into current single project.


FRONTEND :
I HAVE a FRONTEND CHARTING LIB at https://github.com/MaheshUmale/advanced_tvcharts
 

BACKEND:
BACKEND IS IMPLEMENTED at https://github.com/MaheshUmale/unified-app

\tradingview\ is python backend implementation 

We want it to automatically fetch cookies and login using 
 
import rookiepy 
raw_cookies = rookiepy.brave(['.tradingview.com']) 
if raw_cookies: 
    session_token = next((c['value'] for c in raw_cookies if c['name'] == 'sessionid'), None) 
    signature = next((c['value'] for c in raw_cookies if c['name'] == 'sessionid_sign'), None) 
 
 
    os.environ['TV_SESSION'] = session_token 
    os.environ['TV_SIGNATURE'] = signature


