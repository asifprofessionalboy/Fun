SELECT

COMPLAINT_NO,
COMPLAINT_DATE,
VENDOR_CODE,
VENDOR_NAME,
PROBLEM_STATMT,
PROC_CAT_DESC,
COMPAINT_CAT_DESC



from App_COMPLAINT_HELP_REGISTER where VENDOR_CODE = '10104' order by CREATED_ON Desc



Select COMPLAINT_NO,COMPLAINT_DATE,FBACK_JUSCO,FBACK_JUSCODATE,SPL_COMMENT_JUSCO,SPL_COM_JUSCODATE,FBACK_BY_VENDOR,FBACK_BY_VENDDATE
from App_COMPLAINT_HELP_DETAILS where MasterID in (Select ID from App_COMPLAINT_HELP_REGISTER where VENDOR_CODE = '10104')
order by COMPLAINT_NO


I want to join both
