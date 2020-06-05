# SQL_Order_By
Sorted Data


    CREATE ROCEDURE `uspUserSetting`(
      userId int
    )
    BEGIN

       select as.UId, as.JoinTime, 
          as.PhoneNumber, as.Gender,
          as.Nationality, as.EmailAddr,
          as.DepositLevel, as.TopUpAmount
        from app_setting as as
        where as.UId = userId
        order by TableId Asc;

        /* this sp is created by Vivy on 2020.0605 */
        /* add sorted feature on 2020.0605 */

    END
