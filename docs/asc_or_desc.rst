How to order a queryset in ascending or descending order?
=============================================================

Ordering of the queryset can be achieved by order_by method. We need to pass the field on whose basis we need to Order (ascending/descending) the result.
Query looks like this ::

    >>> User.objects.all().order_by('date_joined') // For ascending
    <QuerySet [<User: yash>, <User: John>, <User: Ricky>, <User: sharukh>, <User: Ritesh>, <User: Billy>, <User: Radha>, <User: Raghu>, <User: rishab>, <User: johny>, <User: paul>, <User: johny1>, <User: alien>]>
    >>> User.objects.all().order_by('-date_joined') // For descending; Not '-' sign in order_by method
    <QuerySet [<User: alien>, <User: johny1>, <User: paul>, <User: johny>, <User: rishab>, <User: Raghu>, <User: Radha>, <User: Billy>, <User: Ritesh>, <User: sharukh>, <User: Ricky>, <User: John>, <User: yash>]>
