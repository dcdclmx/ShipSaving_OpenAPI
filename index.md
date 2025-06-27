    Welcome to the ShipSaving Open API documentation.

    This API allows you to:
    - Create and manage orders
    - Retrieve shipping rates
    - Purchase and void shipping labels
    - Generate SCAN forms for USPS and DHL
    - Access account and carrier information
    
    ##  API Integration Flow
    ### 👍 Option 1:
    1. Check Label Pricing List
    2. Purchase Label
    
    ### Option 2:
    💡Limitation about this option: This interface is only applicable to you just have one same type carrier account, like one UPS account, one FEDEX account, one USPS account
    1. Directly Buy Label

    ### Option 3 
    💡Creating orders to our system is not required, you can keep your orders in your system
    1. Create Orders
    2. Check Label Pricing List
    3. Purchase Label
    
    
    ## API Access
    1. Log in to the ShipSaving system. Navigate to **Settings > General**, then click **Renew API Token**. 
        
        💡 Be sure to save the newly generated token, as the previous token will become invalid once a new one is created.
    2. Token settings page: https://s.shipsaving.com/settings/general
    3. ShipSaving provides a RESTful API that uses JSON as both the input and output format.
    

    
    ## Appendix
   

    _Last updated: 2025-06-17_