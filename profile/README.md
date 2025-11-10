## object-detection-model
* Purpose: run inference, send detection events/results
* Separate instance because: GPU variations across machines
* It will call or POST to the main appor write to BaaS

## mobile-application
* Purpose: frontend UX for users
* Talks to: platform via webhooks
, 
## platform
This one holds: 
   * API (for mobile + future web)
   * business logic (detections → violations → notifications)
   * integration with Supabase (BaaS)
