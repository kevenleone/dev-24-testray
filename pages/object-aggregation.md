---
title: Object Aggregation
---

# Object Aggregation

Aggregation is the task of collecting a set of values to return a single one. It is done with the help of functions, such as SUM, COUNT, and AVG.

<img class="flex justify-center" width="700" height="200" src="assets/task-progressbar.png" />

Having this image as example, we need to create an aggregation for each column in **Testray Task Object**

<div m="-t-5" class="aggregation-table">

|                   |       |     |     |
| ---               | ---   | --- | --- |
| NAME              | FIELD | FUNCTION  | FILTER 
| TOTAL COMPLETED   | Score | SUM       | Status = PickList.COMPLETE
| TOTAL             | Score | SUM       | 
| SELF COMPLETED    | Score | SUM       | Status = PickList.COMPLETE & UserID = MyID
| OTHERS COMPLETED  | Score | SUM       | Status = PickList.COMPLETE & UserID != MyID
| INCOMPLETE        | Score | SUM       | Status != PickList.COMPLETE

</div>

<style>
    .aggregation-table {
        margin-top: -10px;
        font-size: 12px;
    }
</style>

