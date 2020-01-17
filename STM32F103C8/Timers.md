Right after you configure a timer - you have to rise update event (UEV). You can do it bu setting UG bit in TIMx_EGR register. 
That event is required for Prescaler (and some other configs) to take effect. If you won't do it, Prescaler won't be used until timer overflows (underflows). So if you use that timer before that overflows happen - it won't be configured with a Prescaler.

To be continued...
