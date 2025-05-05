# Dozen Diamonds API Documentation (UAT)

## POST APIs

1. **Generate Token**  
   `POST https://uat.dozendiamonds.com/user/generateToken/`

2. **Login**  
   `POST https://uat.dozendiamonds.com/user/login/`

3. **Validate MPIN**  
   `POST https://uat.dozendiamonds.com/user/validateMpin/`

4. **Add Funds**  
   `POST https://uat.dozendiamonds.com/api/v1/user/908/account/addfunds`

5. **Past Data Check**  
   `POST https://uat.dozendiamonds.com/api/v1/user/908/past-data-check`

6. **Add Select Stocks**  
   `POST https://uat.dozendiamonds.com/api/v1/user/908/selected-stock/add`

7. **Recommend Parameters of a Stock**  
   `POST https://uat.dozendiamonds.com/api/v1/user/908/stock-recommendation/parameters`

8. **Ladder Creation Parameters**  
   `POST https://uat.dozendiamonds.com/api/v1/user/908/ladder-creation-ticker/fetch`

9. **Past Data**  
   `POST https://uat.dozendiamonds.com/api/v1/user/908/past-data`

10. **Create Ladder**  
    `POST https://uat.dozendiamonds.com/api/v1/user/908/ladder/create`

11. **Add Cash to Ladder**  
    `POST https://uat.dozendiamonds.com/api/v1/user/908/ladder/add-cash`

12. **Withdraw Cash from Ladder**  
    `POST https://uat.dozendiamonds.com/api/v1/user/908/ladder/withdraw-cash`

13. **Merge Ladder**  
    `POST https://uat.dozendiamonds.com/api/v1/user/908/ladder/merge`

14. **Analytics Ticker**  
    `POST https://uat.dozendiamonds.com/api/v1/user/908/analytics`

15. **Withdraw Extra Cash**  
    `POST https://uat.dozendiamonds.com/api/v1/user/:id/withdrawFunds/avaliable-cash`  
    **Request Body:**
    ```json
    {
        "trading_mode": "SIMULATION-PAPER",
        "cash_to_withdraw": 10
    }
    ```

16. **Withdraw Available Cash**  
    `POST https://uat.dozendiamonds.com/api/v1/user/:id/withdrawFunds/avaliable-cash`  
    **Request Body:**
    ```json
    {
        "trading_mode": "SIMULATION-PAPER",
        "cash_to_withdraw": 10
    }
    ```

## GET APIs

1. **Account Details Fetch**  
   `GET https://uat.dozendiamonds.com/api/v1/user/3200/account-details/fetch`

2. **App Config**  
   `GET https://uat.dozendiamonds.com/api/v1/app/config`

3. **Check CSV Status**  
   `GET https://uat.dozendiamonds.com/user/908/check-csv-status`

4. **Search Stock**  
   `GET https://uat.dozendiamonds.com/api/v1/ticker/search?ticker=&pageNumber=0&sector=&country=India`

5. **Sector List**  
   `GET https://uat.dozendiamonds.com/api/v1/ticker/sector-list`

6. **Fetch All Ladders**  
   `GET https://uat.dozendiamonds.com/api/v1/user/908/ladder-implementation/fetch`

7. **Fetch Active Simulator Tickers**  
   `GET https://uat.dozendiamonds.com/api/v1/user/908/active-simulator-tickers/fetch`

8. **Fetch All Trades**  
   `GET https://uat.dozendiamonds.com/api/v1/user/908/unsettled-trades/fetch-all`

9. **Fetch All Open Orders**  
   `GET https://uat.dozendiamonds.com/api/v1/user/908/order/fetch-all`

10. **Fetch All Open Positions**  
    `GET https://uat.dozendiamonds.com/api/v1/user/908/open-positions/fetch-all`

11. **Fetch All Activity**  
    `GET https://uat.dozendiamonds.com/api/v1/user/908/activity/fetch-all?sortType=Date&sortAs=DESC&levelType=LEVEL1`

12. **Download CSV**  
    - **Ladder CSV**: `GET https://uat.dozendiamonds.com/api/v1/user/908/ladder/downloadCsv`  
    - **Trade CSV**: `GET https://uat.dozendiamonds.com/user/908/activity/trading/downloadCsv`  
    - **Order CSV**: `GET https://uat.dozendiamonds.com/api/v1/user/908/order/downloadCsv`  
    - **Position CSV**: `GET https://uat.dozendiamonds.com/api/v1/user/908/position/downloadCsv`  
    - **Activity CSV**: `GET https://uat.dozendiamonds.com/api/v1/user/908/activity/downloadActivityCsv`

## DELETE APIs

1. **Remove Selected Stock**  
   `DELETE https://uat.dozendiamonds.com/api/v1/user/908/selected-stock/remove`

2. **Reset with Retain Ladders**  
   `DELETE https://uat.dozendiamonds.com/api/v1/user/908/account/reset-retain-ladder`

3. **Reset Account**  
   `DELETE https://uat.dozendiamonds.com/api/v1/user/908/account/reset`

## PATCH APIs

1. **Start/Stop Trading**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder/start-stop-trading`

2. **Update All Ladder Status**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder-implementation/update-status/all-ladders`

3. **Update Ladder Status**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder-implementation/update-status`

4. **Update Target Price**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder/update/ladder-target-price`

5. **Update Step Size**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder/update/ladder-stepSize`

6. **Update Order Size**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder/update/ladder-orderSize`

7. **Move Funds to Ladder**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder/update/move-funds-to-ladder`

8. **Make Cash Empty**  
   `PATCH https://uat.dozendiamonds.com/api/v1/user/908/ladder/update/make-cash-empty`

## PUT APIs

1. **Switch Trading Mode**  
   `PUT https://uat.dozendiamonds.com/api/v1/user/908/settings/switch-trading-mode`
