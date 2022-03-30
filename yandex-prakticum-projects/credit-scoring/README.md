{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {
    "toc": true
   },
   "source": [
    "<h1>Содержание<span class=\"tocSkip\"></span></h1>\n",
    "<div class=\"toc\"><ul class=\"toc-item\"></ul></div>"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Описание проекта #\n",
    "\n",
    "Необходимо построить модель прогнозирования ухода клиента из бынка. Предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.\n",
    "\n",
    "Постройте модель с предельно большим значением F1-меры. Нужно довести метрику до 0.59. Проверьте F1-меру на тестовой выборке самостоятельно.\n",
    "\n",
    "Дополнительно измеряйте AUC-ROC, сравнивайте её значение с F1-мерой.\n",
    "\n",
    "**Инструкция по выполнению проекта**\n",
    "\n",
    "1. Загрузите и подготовьте данные. Поясните порядок действий.\n",
    "2. Исследуйте баланс классов, обучите модель без учёта дисбаланса. Кратко опишите выводы.\n",
    "3. Улучшите качество модели, учитывая дисбаланс классов. Обучите разные модели и найдите лучшую. Кратко опишите выводы.\n",
    "4. Проведите финальное тестирование.\n",
    "\n",
    "**Описание данных**\n",
    "\n",
    "    RowNumber — индекс строки в данных\n",
    "    CustomerId — уникальный идентификатор клиента\n",
    "    Surname — фамилия\n",
    "    CreditScore — кредитный рейтинг\n",
    "    Geography — страна проживания\n",
    "    Gender — пол\n",
    "    Age — возраст\n",
    "    Tenure — сколько лет человек является клиентом банка\n",
    "    Balance — баланс на счёте\n",
    "    NumOfProducts — количество продуктов банка, используемых клиентом\n",
    "    HasCrCard — наличие кредитной карты\n",
    "    IsActiveMember — активность клиента\n",
    "    EstimatedSalary — предполагаемая зарплата\n",
    "\n",
    "**Целевой признак**\n",
    "\n",
    "    Exited — факт ухода клиента    "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**Вывод**\n",
    "\n",
    "После всех манипуляций с моделями, удалось получить F1=0,5989 на тестовой выборке, что говорит о достаточном уровне предсказаний модели бустинга."
   ]
  }
 ],
 "metadata": {
  "ExecuteTimeLog": [
   {
    "duration": 765,
    "start_time": "2022-02-22T09:38:24.816Z"
   },
   {
    "duration": 5913,
    "start_time": "2022-02-22T09:38:53.138Z"
   },
   {
    "duration": 6169,
    "start_time": "2022-02-22T09:44:07.129Z"
   },
   {
    "duration": 177,
    "start_time": "2022-02-22T09:45:49.217Z"
   },
   {
    "duration": 37,
    "start_time": "2022-02-22T09:48:15.025Z"
   },
   {
    "duration": 63,
    "start_time": "2022-02-22T09:54:44.175Z"
   },
   {
    "duration": 591,
    "start_time": "2022-02-22T10:29:36.668Z"
   },
   {
    "duration": 22,
    "start_time": "2022-02-22T10:35:10.322Z"
   },
   {
    "duration": 40,
    "start_time": "2022-02-22T10:36:25.178Z"
   },
   {
    "duration": 37,
    "start_time": "2022-02-22T10:37:09.684Z"
   },
   {
    "duration": 44,
    "start_time": "2022-02-22T10:37:50.221Z"
   },
   {
    "duration": 367,
    "start_time": "2022-02-22T10:38:24.939Z"
   },
   {
    "duration": 44,
    "start_time": "2022-02-22T10:38:44.411Z"
   },
   {
    "duration": 52,
    "start_time": "2022-02-22T10:39:03.093Z"
   },
   {
    "duration": 64,
    "start_time": "2022-02-22T10:40:14.187Z"
   },
   {
    "duration": 122,
    "start_time": "2022-02-22T10:40:39.441Z"
   },
   {
    "duration": 22,
    "start_time": "2022-02-22T10:40:56.602Z"
   },
   {
    "duration": 57,
    "start_time": "2022-02-22T10:43:00.730Z"
   },
   {
    "duration": 507,
    "start_time": "2022-02-22T10:43:49.833Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-22T10:45:03.419Z"
   },
   {
    "duration": 327,
    "start_time": "2022-02-22T10:48:01.248Z"
   },
   {
    "duration": 26,
    "start_time": "2022-02-22T10:48:21.132Z"
   },
   {
    "duration": 20,
    "start_time": "2022-02-22T10:48:30.761Z"
   },
   {
    "duration": 329,
    "start_time": "2022-02-22T10:48:52.105Z"
   },
   {
    "duration": 1683,
    "start_time": "2022-02-22T10:49:17.830Z"
   },
   {
    "duration": 83,
    "start_time": "2022-02-22T10:49:20.517Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-22T10:49:24.437Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-22T10:50:28.454Z"
   },
   {
    "duration": 10053,
    "start_time": "2022-02-22T10:51:40.901Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-22T10:52:12.502Z"
   },
   {
    "duration": 7593,
    "start_time": "2022-02-22T10:54:51.813Z"
   },
   {
    "duration": 292,
    "start_time": "2022-02-22T10:57:45.989Z"
   },
   {
    "duration": 496,
    "start_time": "2022-02-22T10:58:14.325Z"
   },
   {
    "duration": 7236,
    "start_time": "2022-02-22T10:58:23.221Z"
   },
   {
    "duration": 7117,
    "start_time": "2022-02-22T10:58:32.775Z"
   },
   {
    "duration": -130,
    "start_time": "2022-02-22T10:58:51.650Z"
   },
   {
    "duration": 89,
    "start_time": "2022-02-22T10:58:55.461Z"
   },
   {
    "duration": 310,
    "start_time": "2022-02-22T10:59:06.629Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-22T11:00:17.461Z"
   },
   {
    "duration": 22,
    "start_time": "2022-02-22T11:00:27.369Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-22T11:01:31.132Z"
   },
   {
    "duration": 348,
    "start_time": "2022-02-22T11:02:00.293Z"
   },
   {
    "duration": 1425,
    "start_time": "2022-02-22T11:02:25.067Z"
   },
   {
    "duration": 73,
    "start_time": "2022-02-22T11:02:26.495Z"
   },
   {
    "duration": 20,
    "start_time": "2022-02-22T11:02:33.129Z"
   },
   {
    "duration": 22,
    "start_time": "2022-02-22T11:02:34.281Z"
   },
   {
    "duration": 1466,
    "start_time": "2022-02-22T11:03:35.319Z"
   },
   {
    "duration": 63,
    "start_time": "2022-02-22T11:03:37.430Z"
   },
   {
    "duration": 21,
    "start_time": "2022-02-22T11:03:42.773Z"
   },
   {
    "duration": 46,
    "start_time": "2022-02-22T11:04:16.885Z"
   },
   {
    "duration": 1339,
    "start_time": "2022-02-22T11:11:56.043Z"
   },
   {
    "duration": 65,
    "start_time": "2022-02-22T11:11:57.850Z"
   },
   {
    "duration": 17,
    "start_time": "2022-02-22T11:12:01.065Z"
   },
   {
    "duration": 36,
    "start_time": "2022-02-22T11:12:09.545Z"
   },
   {
    "duration": 21,
    "start_time": "2022-02-22T11:12:37.737Z"
   },
   {
    "duration": 23,
    "start_time": "2022-02-22T11:12:48.905Z"
   },
   {
    "duration": 431,
    "start_time": "2022-02-22T11:13:38.889Z"
   },
   {
    "duration": 451,
    "start_time": "2022-02-22T11:16:11.082Z"
   },
   {
    "duration": 1328,
    "start_time": "2022-02-22T11:16:21.628Z"
   },
   {
    "duration": 66,
    "start_time": "2022-02-22T11:16:22.959Z"
   },
   {
    "duration": 27,
    "start_time": "2022-02-22T11:16:23.028Z"
   },
   {
    "duration": 34,
    "start_time": "2022-02-22T11:16:23.057Z"
   },
   {
    "duration": 20,
    "start_time": "2022-02-22T11:16:23.093Z"
   },
   {
    "duration": 653,
    "start_time": "2022-02-22T11:16:23.116Z"
   },
   {
    "duration": 323,
    "start_time": "2022-02-22T11:16:40.579Z"
   },
   {
    "duration": 364,
    "start_time": "2022-02-22T11:17:05.651Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-22T11:17:14.307Z"
   },
   {
    "duration": 291,
    "start_time": "2022-02-22T11:17:44.003Z"
   },
   {
    "duration": 1131,
    "start_time": "2022-02-24T07:30:47.413Z"
   },
   {
    "duration": 47,
    "start_time": "2022-02-24T07:30:48.545Z"
   },
   {
    "duration": 25,
    "start_time": "2022-02-24T07:30:48.594Z"
   },
   {
    "duration": 25,
    "start_time": "2022-02-24T07:30:48.621Z"
   },
   {
    "duration": 16,
    "start_time": "2022-02-24T07:30:48.648Z"
   },
   {
    "duration": 305,
    "start_time": "2022-02-24T07:30:48.666Z"
   },
   {
    "duration": 14,
    "start_time": "2022-02-24T07:37:51.135Z"
   },
   {
    "duration": 14,
    "start_time": "2022-02-24T07:38:05.445Z"
   },
   {
    "duration": 26,
    "start_time": "2022-02-24T07:38:08.756Z"
   },
   {
    "duration": 240,
    "start_time": "2022-02-24T10:20:15.917Z"
   },
   {
    "duration": 3,
    "start_time": "2022-02-24T10:20:27.654Z"
   },
   {
    "duration": 33,
    "start_time": "2022-02-24T10:20:30.888Z"
   },
   {
    "duration": 3,
    "start_time": "2022-02-24T10:26:37.380Z"
   },
   {
    "duration": 1136,
    "start_time": "2022-02-24T10:27:00.111Z"
   },
   {
    "duration": 49,
    "start_time": "2022-02-24T10:27:01.249Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-24T10:27:01.300Z"
   },
   {
    "duration": 21,
    "start_time": "2022-02-24T10:27:01.321Z"
   },
   {
    "duration": 14,
    "start_time": "2022-02-24T10:27:01.344Z"
   },
   {
    "duration": 18,
    "start_time": "2022-02-24T10:27:01.359Z"
   },
   {
    "duration": 3,
    "start_time": "2022-02-24T11:50:50.944Z"
   },
   {
    "duration": 26,
    "start_time": "2022-02-24T11:51:48.622Z"
   },
   {
    "duration": 24,
    "start_time": "2022-02-24T11:55:02.574Z"
   },
   {
    "duration": 413,
    "start_time": "2022-02-24T11:58:54.940Z"
   },
   {
    "duration": 25,
    "start_time": "2022-02-24T11:59:09.694Z"
   },
   {
    "duration": 264,
    "start_time": "2022-02-24T12:02:07.196Z"
   },
   {
    "duration": 390,
    "start_time": "2022-02-24T12:02:33.196Z"
   },
   {
    "duration": 98,
    "start_time": "2022-02-24T12:02:51.821Z"
   },
   {
    "duration": 92,
    "start_time": "2022-02-24T12:03:06.429Z"
   },
   {
    "duration": 397,
    "start_time": "2022-02-24T12:04:22.970Z"
   },
   {
    "duration": 3,
    "start_time": "2022-02-24T12:04:49.355Z"
   },
   {
    "duration": 104,
    "start_time": "2022-02-24T12:04:53.515Z"
   },
   {
    "duration": 1051,
    "start_time": "2022-02-24T18:16:13.490Z"
   },
   {
    "duration": 47,
    "start_time": "2022-02-24T18:16:14.543Z"
   },
   {
    "duration": 10,
    "start_time": "2022-02-24T18:16:14.592Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-24T18:16:14.603Z"
   },
   {
    "duration": 13,
    "start_time": "2022-02-24T18:16:14.632Z"
   },
   {
    "duration": 96,
    "start_time": "2022-02-24T18:16:14.646Z"
   },
   {
    "duration": 23,
    "start_time": "2022-02-24T18:26:34.547Z"
   },
   {
    "duration": 5,
    "start_time": "2022-02-24T18:29:21.659Z"
   },
   {
    "duration": 8,
    "start_time": "2022-02-24T18:33:11.078Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-24T18:33:34.446Z"
   },
   {
    "duration": 195,
    "start_time": "2022-02-24T18:35:36.847Z"
   },
   {
    "duration": 395,
    "start_time": "2022-02-24T18:36:58.846Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-24T18:37:30.495Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-24T18:37:48.783Z"
   },
   {
    "duration": 311,
    "start_time": "2022-02-24T18:38:00.678Z"
   },
   {
    "duration": 337,
    "start_time": "2022-02-24T18:38:19.902Z"
   },
   {
    "duration": 368,
    "start_time": "2022-02-24T18:42:53.855Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-24T18:43:07.848Z"
   },
   {
    "duration": 5,
    "start_time": "2022-02-24T18:43:20.215Z"
   },
   {
    "duration": 292,
    "start_time": "2022-02-24T18:43:29.287Z"
   },
   {
    "duration": 5,
    "start_time": "2022-02-24T18:44:53.200Z"
   },
   {
    "duration": 318,
    "start_time": "2022-02-24T18:46:58.280Z"
   },
   {
    "duration": 70,
    "start_time": "2022-02-24T18:47:16.336Z"
   },
   {
    "duration": 436,
    "start_time": "2022-02-24T18:47:20.304Z"
   },
   {
    "duration": 433,
    "start_time": "2022-02-24T18:47:51.240Z"
   },
   {
    "duration": 664,
    "start_time": "2022-02-24T18:49:26.320Z"
   },
   {
    "duration": 11309,
    "start_time": "2022-02-24T18:49:51.665Z"
   },
   {
    "duration": 474,
    "start_time": "2022-02-24T18:50:20.352Z"
   },
   {
    "duration": 7,
    "start_time": "2022-02-24T18:50:28.968Z"
   },
   {
    "duration": 670,
    "start_time": "2022-02-24T18:55:16.385Z"
   },
   {
    "duration": 526,
    "start_time": "2022-02-24T18:56:52.537Z"
   },
   {
    "duration": 703,
    "start_time": "2022-02-24T18:57:32.610Z"
   },
   {
    "duration": 175,
    "start_time": "2022-02-24T18:59:05.290Z"
   },
   {
    "duration": 176,
    "start_time": "2022-02-24T19:00:13.475Z"
   },
   {
    "duration": 1507,
    "start_time": "2022-02-25T06:27:42.189Z"
   },
   {
    "duration": 123,
    "start_time": "2022-02-25T06:27:43.699Z"
   },
   {
    "duration": 15,
    "start_time": "2022-02-25T06:27:43.825Z"
   },
   {
    "duration": 38,
    "start_time": "2022-02-25T06:27:43.843Z"
   },
   {
    "duration": 21,
    "start_time": "2022-02-25T06:27:43.883Z"
   },
   {
    "duration": 155,
    "start_time": "2022-02-25T06:27:43.906Z"
   },
   {
    "duration": 7,
    "start_time": "2022-02-25T06:27:44.065Z"
   },
   {
    "duration": 8,
    "start_time": "2022-02-25T06:27:44.163Z"
   },
   {
    "duration": 370,
    "start_time": "2022-02-25T06:27:44.174Z"
   },
   {
    "duration": 324,
    "start_time": "2022-02-25T06:34:12.786Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-25T06:38:23.106Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-25T06:38:53.058Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-25T08:48:42.151Z"
   },
   {
    "duration": 66,
    "start_time": "2022-02-25T08:48:42.158Z"
   },
   {
    "duration": 17,
    "start_time": "2022-02-25T08:48:42.227Z"
   },
   {
    "duration": 40,
    "start_time": "2022-02-25T08:48:42.247Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-25T08:48:42.290Z"
   },
   {
    "duration": 65,
    "start_time": "2022-02-25T08:48:42.311Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-25T08:48:42.461Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-25T08:48:42.563Z"
   },
   {
    "duration": 345,
    "start_time": "2022-02-25T08:48:42.572Z"
   },
   {
    "duration": 153,
    "start_time": "2022-02-25T09:12:44.010Z"
   },
   {
    "duration": 23,
    "start_time": "2022-02-25T09:47:45.040Z"
   },
   {
    "duration": 97,
    "start_time": "2022-02-25T09:48:29.777Z"
   },
   {
    "duration": 61,
    "start_time": "2022-02-25T09:48:43.733Z"
   },
   {
    "duration": 57,
    "start_time": "2022-02-25T09:49:00.090Z"
   },
   {
    "duration": 606,
    "start_time": "2022-02-25T09:49:24.847Z"
   },
   {
    "duration": 323,
    "start_time": "2022-02-25T09:49:42.689Z"
   },
   {
    "duration": 309,
    "start_time": "2022-02-25T09:51:37.519Z"
   },
   {
    "duration": 14,
    "start_time": "2022-02-25T09:51:42.351Z"
   },
   {
    "duration": 128,
    "start_time": "2022-02-25T09:51:47.649Z"
   },
   {
    "duration": 1067,
    "start_time": "2022-02-25T09:52:39.136Z"
   },
   {
    "duration": 504,
    "start_time": "2022-02-25T10:01:02.206Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-25T10:01:37.774Z"
   },
   {
    "duration": 138,
    "start_time": "2022-02-25T10:01:43.823Z"
   },
   {
    "duration": 152,
    "start_time": "2022-02-25T10:02:26.016Z"
   },
   {
    "duration": 312,
    "start_time": "2022-02-25T10:02:59.949Z"
   },
   {
    "duration": 107,
    "start_time": "2022-02-25T10:03:08.206Z"
   },
   {
    "duration": 2338,
    "start_time": "2022-02-25T10:03:55.326Z"
   },
   {
    "duration": 310,
    "start_time": "2022-02-25T10:09:59.261Z"
   },
   {
    "duration": 306,
    "start_time": "2022-02-25T10:10:13.758Z"
   },
   {
    "duration": 292,
    "start_time": "2022-02-25T10:10:54.413Z"
   },
   {
    "duration": 8,
    "start_time": "2022-02-25T10:11:20.461Z"
   },
   {
    "duration": 100,
    "start_time": "2022-02-25T10:11:37.262Z"
   },
   {
    "duration": 70,
    "start_time": "2022-02-25T10:11:38.606Z"
   },
   {
    "duration": 1684,
    "start_time": "2022-02-25T10:11:39.277Z"
   },
   {
    "duration": 85896,
    "start_time": "2022-02-25T10:27:53.606Z"
   },
   {
    "duration": 143999,
    "start_time": "2022-02-25T10:29:21.294Z"
   },
   {
    "duration": 698,
    "start_time": "2022-02-25T10:32:16.828Z"
   },
   {
    "duration": 753,
    "start_time": "2022-02-25T10:33:14.914Z"
   },
   {
    "duration": 1454,
    "start_time": "2022-02-25T10:33:51.667Z"
   },
   {
    "duration": 65,
    "start_time": "2022-02-25T10:33:53.125Z"
   },
   {
    "duration": 16,
    "start_time": "2022-02-25T10:33:53.193Z"
   },
   {
    "duration": 60,
    "start_time": "2022-02-25T10:33:53.212Z"
   },
   {
    "duration": 20,
    "start_time": "2022-02-25T10:33:53.274Z"
   },
   {
    "duration": 68,
    "start_time": "2022-02-25T10:33:53.297Z"
   },
   {
    "duration": 94,
    "start_time": "2022-02-25T10:33:53.369Z"
   },
   {
    "duration": 8,
    "start_time": "2022-02-25T10:33:53.467Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-25T10:33:53.478Z"
   },
   {
    "duration": 362,
    "start_time": "2022-02-25T10:33:53.487Z"
   },
   {
    "duration": 119,
    "start_time": "2022-02-25T10:33:53.852Z"
   },
   {
    "duration": 229,
    "start_time": "2022-02-25T10:33:53.975Z"
   },
   {
    "duration": 1126,
    "start_time": "2022-02-25T10:33:54.206Z"
   },
   {
    "duration": 138,
    "start_time": "2022-02-25T10:33:55.334Z"
   },
   {
    "duration": 122,
    "start_time": "2022-02-25T10:33:55.562Z"
   },
   {
    "duration": 1589,
    "start_time": "2022-02-25T10:33:55.686Z"
   },
   {
    "duration": 968,
    "start_time": "2022-02-25T10:33:57.278Z"
   },
   {
    "duration": -53,
    "start_time": "2022-02-25T10:33:58.302Z"
   },
   {
    "duration": 1590,
    "start_time": "2022-02-25T10:51:25.278Z"
   },
   {
    "duration": 73,
    "start_time": "2022-02-25T10:52:14.055Z"
   },
   {
    "duration": 72,
    "start_time": "2022-02-25T10:52:22.648Z"
   },
   {
    "duration": 76,
    "start_time": "2022-02-25T10:52:58.536Z"
   },
   {
    "duration": 1659,
    "start_time": "2022-02-25T10:52:59.975Z"
   },
   {
    "duration": 58,
    "start_time": "2022-02-25T10:53:53.289Z"
   },
   {
    "duration": 171,
    "start_time": "2022-02-25T10:54:44.106Z"
   },
   {
    "duration": 1664,
    "start_time": "2022-02-25T10:55:58.219Z"
   },
   {
    "duration": 2049,
    "start_time": "2022-02-25T10:56:22.103Z"
   },
   {
    "duration": 1658,
    "start_time": "2022-02-25T10:56:32.856Z"
   },
   {
    "duration": 70,
    "start_time": "2022-02-25T10:56:46.218Z"
   },
   {
    "duration": 103,
    "start_time": "2022-02-25T10:56:51.560Z"
   },
   {
    "duration": 1108,
    "start_time": "2022-02-25T10:56:58.135Z"
   },
   {
    "duration": 58,
    "start_time": "2022-02-25T10:57:05.654Z"
   },
   {
    "duration": 96,
    "start_time": "2022-02-25T10:57:10.791Z"
   },
   {
    "duration": 1525,
    "start_time": "2022-02-25T11:43:04.799Z"
   },
   {
    "duration": 122,
    "start_time": "2022-02-25T11:43:06.326Z"
   },
   {
    "duration": 16,
    "start_time": "2022-02-25T11:43:06.451Z"
   },
   {
    "duration": 33,
    "start_time": "2022-02-25T11:43:06.470Z"
   },
   {
    "duration": 22,
    "start_time": "2022-02-25T11:43:06.506Z"
   },
   {
    "duration": 137,
    "start_time": "2022-02-25T11:43:06.530Z"
   },
   {
    "duration": 97,
    "start_time": "2022-02-25T11:43:06.670Z"
   },
   {
    "duration": 8,
    "start_time": "2022-02-25T11:43:06.769Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-25T11:43:06.781Z"
   },
   {
    "duration": 374,
    "start_time": "2022-02-25T11:43:06.790Z"
   },
   {
    "duration": 101,
    "start_time": "2022-02-25T11:43:07.167Z"
   },
   {
    "duration": 240,
    "start_time": "2022-02-25T11:43:07.272Z"
   },
   {
    "duration": 1084,
    "start_time": "2022-02-25T11:43:07.514Z"
   },
   {
    "duration": 80,
    "start_time": "2022-02-25T11:43:08.601Z"
   },
   {
    "duration": 162,
    "start_time": "2022-02-25T11:43:08.763Z"
   },
   {
    "duration": 1752,
    "start_time": "2022-02-25T11:43:08.928Z"
   },
   {
    "duration": 112,
    "start_time": "2022-02-25T11:43:10.683Z"
   },
   {
    "duration": 151,
    "start_time": "2022-02-25T11:43:10.863Z"
   },
   {
    "duration": 1745,
    "start_time": "2022-02-25T11:43:11.017Z"
   },
   {
    "duration": -152,
    "start_time": "2022-02-25T11:48:37.431Z"
   },
   {
    "duration": 1496,
    "start_time": "2022-02-25T11:50:32.733Z"
   },
   {
    "duration": 121,
    "start_time": "2022-02-25T11:50:34.233Z"
   },
   {
    "duration": 14,
    "start_time": "2022-02-25T11:50:34.360Z"
   },
   {
    "duration": 36,
    "start_time": "2022-02-25T11:50:34.377Z"
   },
   {
    "duration": 18,
    "start_time": "2022-02-25T11:50:34.415Z"
   },
   {
    "duration": 53,
    "start_time": "2022-02-25T11:50:34.435Z"
   },
   {
    "duration": 9,
    "start_time": "2022-02-25T11:50:34.562Z"
   },
   {
    "duration": 8,
    "start_time": "2022-02-25T11:50:34.663Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-25T11:50:34.674Z"
   },
   {
    "duration": 359,
    "start_time": "2022-02-25T11:50:34.682Z"
   },
   {
    "duration": 119,
    "start_time": "2022-02-25T11:50:35.044Z"
   },
   {
    "duration": 215,
    "start_time": "2022-02-25T11:50:35.166Z"
   },
   {
    "duration": 1064,
    "start_time": "2022-02-25T11:50:35.383Z"
   },
   {
    "duration": 123,
    "start_time": "2022-02-25T11:50:36.450Z"
   },
   {
    "duration": 168,
    "start_time": "2022-02-25T11:50:36.577Z"
   },
   {
    "duration": 1594,
    "start_time": "2022-02-25T11:50:36.762Z"
   },
   {
    "duration": 212382,
    "start_time": "2022-02-25T11:50:38.360Z"
   },
   {
    "duration": 123,
    "start_time": "2022-02-25T11:54:10.744Z"
   },
   {
    "duration": 235,
    "start_time": "2022-02-25T11:54:10.870Z"
   },
   {
    "duration": 1621,
    "start_time": "2022-02-25T11:54:11.107Z"
   },
   {
    "duration": 65,
    "start_time": "2022-02-25T11:54:37.957Z"
   },
   {
    "duration": 5,
    "start_time": "2022-02-25T11:55:28.437Z"
   },
   {
    "duration": 514,
    "start_time": "2022-02-25T11:58:03.845Z"
   },
   {
    "duration": 5,
    "start_time": "2022-02-25T11:58:16.745Z"
   },
   {
    "duration": 392,
    "start_time": "2022-02-25T11:58:23.220Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-25T11:58:40.260Z"
   },
   {
    "duration": 319,
    "start_time": "2022-02-25T11:58:45.667Z"
   },
   {
    "duration": 1236,
    "start_time": "2022-02-26T17:42:25.961Z"
   },
   {
    "duration": 39,
    "start_time": "2022-02-26T17:42:27.199Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-26T17:42:27.240Z"
   },
   {
    "duration": 21,
    "start_time": "2022-02-26T17:42:27.263Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-26T17:42:27.286Z"
   },
   {
    "duration": 163,
    "start_time": "2022-02-26T17:42:27.300Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-26T17:42:27.465Z"
   },
   {
    "duration": 14,
    "start_time": "2022-02-26T17:42:27.473Z"
   },
   {
    "duration": 10,
    "start_time": "2022-02-26T17:42:27.491Z"
   },
   {
    "duration": 338,
    "start_time": "2022-02-26T17:42:27.504Z"
   },
   {
    "duration": 132,
    "start_time": "2022-02-26T17:42:27.844Z"
   },
   {
    "duration": 127,
    "start_time": "2022-02-26T17:42:27.978Z"
   },
   {
    "duration": 780,
    "start_time": "2022-02-26T17:42:28.107Z"
   },
   {
    "duration": 82,
    "start_time": "2022-02-26T17:42:28.889Z"
   },
   {
    "duration": 191,
    "start_time": "2022-02-26T17:42:28.973Z"
   },
   {
    "duration": 1608,
    "start_time": "2022-02-26T17:42:29.167Z"
   },
   {
    "duration": 122618,
    "start_time": "2022-02-26T17:42:30.777Z"
   },
   {
    "duration": 464,
    "start_time": "2022-02-26T17:44:32.934Z"
   },
   {
    "duration": 465,
    "start_time": "2022-02-26T17:44:32.935Z"
   },
   {
    "duration": 465,
    "start_time": "2022-02-26T17:44:32.936Z"
   },
   {
    "duration": 466,
    "start_time": "2022-02-26T17:44:32.937Z"
   },
   {
    "duration": 70989,
    "start_time": "2022-02-26T17:45:22.145Z"
   },
   {
    "duration": 564093,
    "start_time": "2022-02-26T17:55:00.415Z"
   },
   {
    "duration": 32071,
    "start_time": "2022-02-26T18:04:48.529Z"
   },
   {
    "duration": 25701,
    "start_time": "2022-02-26T18:06:41.396Z"
   },
   {
    "duration": 213949,
    "start_time": "2022-02-26T18:07:09.005Z"
   },
   {
    "duration": 1580,
    "start_time": "2022-02-26T18:26:08.683Z"
   },
   {
    "duration": 150876,
    "start_time": "2022-02-26T18:30:19.248Z"
   },
   {
    "duration": 66800,
    "start_time": "2022-02-26T18:34:50.488Z"
   },
   {
    "duration": 66684,
    "start_time": "2022-02-26T18:36:13.728Z"
   },
   {
    "duration": 58773,
    "start_time": "2022-02-26T18:39:30.872Z"
   },
   {
    "duration": 67875,
    "start_time": "2022-02-26T18:40:40.296Z"
   },
   {
    "duration": 86937,
    "start_time": "2022-02-26T18:43:23.828Z"
   },
   {
    "duration": 29542,
    "start_time": "2022-02-26T18:46:53.197Z"
   },
   {
    "duration": 29692,
    "start_time": "2022-02-26T18:53:28.082Z"
   },
   {
    "duration": 1399,
    "start_time": "2022-02-26T18:55:10.638Z"
   },
   {
    "duration": 1144,
    "start_time": "2022-02-26T18:56:23.437Z"
   },
   {
    "duration": 1049,
    "start_time": "2022-02-26T18:57:29.658Z"
   },
   {
    "duration": 1987,
    "start_time": "2022-02-26T18:57:44.577Z"
   },
   {
    "duration": 2092,
    "start_time": "2022-02-26T18:59:23.464Z"
   },
   {
    "duration": 106,
    "start_time": "2022-02-26T18:59:25.558Z"
   },
   {
    "duration": 146,
    "start_time": "2022-02-26T18:59:25.667Z"
   },
   {
    "duration": 96,
    "start_time": "2022-02-26T18:59:25.815Z"
   },
   {
    "duration": 166,
    "start_time": "2022-02-26T18:59:25.913Z"
   },
   {
    "duration": 195,
    "start_time": "2022-02-26T19:04:48.603Z"
   },
   {
    "duration": 1323,
    "start_time": "2022-02-26T19:09:21.727Z"
   },
   {
    "duration": 1456,
    "start_time": "2022-02-26T19:09:35.499Z"
   },
   {
    "duration": 2031,
    "start_time": "2022-02-26T19:09:42.138Z"
   },
   {
    "duration": 301,
    "start_time": "2022-02-26T19:10:09.103Z"
   },
   {
    "duration": 898,
    "start_time": "2022-02-26T19:10:32.846Z"
   },
   {
    "duration": 2948,
    "start_time": "2022-02-26T19:10:42.259Z"
   },
   {
    "duration": 95540,
    "start_time": "2022-02-26T19:11:47.003Z"
   },
   {
    "duration": 243,
    "start_time": "2022-02-26T19:13:48.947Z"
   },
   {
    "duration": 54584,
    "start_time": "2022-02-26T19:13:53.723Z"
   },
   {
    "duration": 27817,
    "start_time": "2022-02-26T19:16:32.823Z"
   },
   {
    "duration": 13816,
    "start_time": "2022-02-26T19:17:12.980Z"
   },
   {
    "duration": 67659,
    "start_time": "2022-02-26T19:18:10.076Z"
   },
   {
    "duration": 68439,
    "start_time": "2022-02-26T19:19:26.225Z"
   },
   {
    "duration": 63966,
    "start_time": "2022-02-26T19:20:34.665Z"
   },
   {
    "duration": 30532,
    "start_time": "2022-02-26T19:21:38.633Z"
   },
   {
    "duration": 2046,
    "start_time": "2022-02-26T19:22:09.168Z"
   },
   {
    "duration": 159,
    "start_time": "2022-02-26T19:22:11.216Z"
   },
   {
    "duration": 140,
    "start_time": "2022-02-26T19:22:11.377Z"
   },
   {
    "duration": 56,
    "start_time": "2022-02-26T19:22:11.519Z"
   },
   {
    "duration": 175,
    "start_time": "2022-02-26T19:22:11.576Z"
   },
   {
    "duration": 229,
    "start_time": "2022-02-26T19:23:01.769Z"
   },
   {
    "duration": 1506,
    "start_time": "2022-02-26T19:25:43.422Z"
   },
   {
    "duration": 900,
    "start_time": "2022-02-26T19:28:35.453Z"
   },
   {
    "duration": 892,
    "start_time": "2022-02-26T19:28:45.533Z"
   },
   {
    "duration": 247,
    "start_time": "2022-02-26T19:30:09.830Z"
   },
   {
    "duration": 264,
    "start_time": "2022-02-26T19:30:19.869Z"
   },
   {
    "duration": 3415,
    "start_time": "2022-02-26T19:30:24.990Z"
   },
   {
    "duration": 251,
    "start_time": "2022-02-26T19:31:12.110Z"
   },
   {
    "duration": 809,
    "start_time": "2022-02-26T19:31:23.591Z"
   },
   {
    "duration": 27925,
    "start_time": "2022-02-26T19:34:23.316Z"
   },
   {
    "duration": 88725,
    "start_time": "2022-02-26T19:35:15.694Z"
   },
   {
    "duration": 140242,
    "start_time": "2022-02-26T19:37:32.015Z"
   },
   {
    "duration": 156626,
    "start_time": "2022-02-26T19:40:18.712Z"
   },
   {
    "duration": 133393,
    "start_time": "2022-02-26T19:43:27.936Z"
   },
   {
    "duration": 1294,
    "start_time": "2022-02-26T19:49:27.901Z"
   },
   {
    "duration": 1346,
    "start_time": "2022-02-26T19:50:30.537Z"
   },
   {
    "duration": 1509,
    "start_time": "2022-02-26T19:50:35.688Z"
   },
   {
    "duration": 1526,
    "start_time": "2022-02-26T19:51:18.354Z"
   },
   {
    "duration": 1468,
    "start_time": "2022-02-26T19:51:30.009Z"
   },
   {
    "duration": 6806,
    "start_time": "2022-02-26T19:52:03.009Z"
   },
   {
    "duration": 1187,
    "start_time": "2022-02-28T05:06:53.102Z"
   },
   {
    "duration": 49,
    "start_time": "2022-02-28T05:06:54.291Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-28T05:06:54.342Z"
   },
   {
    "duration": 24,
    "start_time": "2022-02-28T05:06:54.356Z"
   },
   {
    "duration": 15,
    "start_time": "2022-02-28T05:06:54.402Z"
   },
   {
    "duration": 82,
    "start_time": "2022-02-28T05:06:54.419Z"
   },
   {
    "duration": 97,
    "start_time": "2022-02-28T05:06:54.504Z"
   },
   {
    "duration": 7,
    "start_time": "2022-02-28T05:06:54.604Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-28T05:06:54.613Z"
   },
   {
    "duration": 229,
    "start_time": "2022-02-28T05:06:54.621Z"
   },
   {
    "duration": 149,
    "start_time": "2022-02-28T05:06:54.852Z"
   },
   {
    "duration": 134,
    "start_time": "2022-02-28T05:06:55.006Z"
   },
   {
    "duration": 792,
    "start_time": "2022-02-28T05:06:55.142Z"
   },
   {
    "duration": 167,
    "start_time": "2022-02-28T05:06:55.936Z"
   },
   {
    "duration": 129,
    "start_time": "2022-02-28T05:06:56.105Z"
   },
   {
    "duration": 1126,
    "start_time": "2022-02-28T05:06:56.237Z"
   },
   {
    "duration": 1129,
    "start_time": "2022-02-28T05:06:57.365Z"
   },
   {
    "duration": 69282,
    "start_time": "2022-02-28T05:06:58.501Z"
   },
   {
    "duration": 63318,
    "start_time": "2022-02-28T05:08:07.785Z"
   },
   {
    "duration": 30628,
    "start_time": "2022-02-28T05:09:11.105Z"
   },
   {
    "duration": 1408,
    "start_time": "2022-02-28T05:09:41.735Z"
   },
   {
    "duration": 7202,
    "start_time": "2022-02-28T05:09:43.145Z"
   },
   {
    "duration": 157,
    "start_time": "2022-02-28T05:09:50.350Z"
   },
   {
    "duration": 128,
    "start_time": "2022-02-28T05:09:50.509Z"
   },
   {
    "duration": 65,
    "start_time": "2022-02-28T05:09:50.639Z"
   },
   {
    "duration": 178,
    "start_time": "2022-02-28T05:09:50.706Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-28T05:14:54.606Z"
   },
   {
    "duration": 427,
    "start_time": "2022-02-28T05:16:23.802Z"
   },
   {
    "duration": 38802,
    "start_time": "2022-02-28T05:50:17.078Z"
   },
   {
    "duration": 307,
    "start_time": "2022-02-28T06:01:43.781Z"
   },
   {
    "duration": 252,
    "start_time": "2022-02-28T06:03:50.228Z"
   },
   {
    "duration": 205,
    "start_time": "2022-02-28T06:04:06.726Z"
   },
   {
    "duration": 155299,
    "start_time": "2022-02-28T06:05:10.809Z"
   },
   {
    "duration": 136734,
    "start_time": "2022-02-28T06:07:51.268Z"
   },
   {
    "duration": 1251,
    "start_time": "2022-02-28T06:36:37.403Z"
   },
   {
    "duration": 49,
    "start_time": "2022-02-28T06:36:38.657Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-28T06:36:38.709Z"
   },
   {
    "duration": 26,
    "start_time": "2022-02-28T06:36:38.723Z"
   },
   {
    "duration": 16,
    "start_time": "2022-02-28T06:36:38.751Z"
   },
   {
    "duration": 136,
    "start_time": "2022-02-28T06:36:38.769Z"
   },
   {
    "duration": 94,
    "start_time": "2022-02-28T06:36:38.909Z"
   },
   {
    "duration": 9,
    "start_time": "2022-02-28T06:36:39.006Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-28T06:36:39.018Z"
   },
   {
    "duration": 228,
    "start_time": "2022-02-28T06:36:39.032Z"
   },
   {
    "duration": 65,
    "start_time": "2022-02-28T06:36:39.262Z"
   },
   {
    "duration": 200,
    "start_time": "2022-02-28T06:36:39.329Z"
   },
   {
    "duration": 828,
    "start_time": "2022-02-28T06:36:39.531Z"
   },
   {
    "duration": 55,
    "start_time": "2022-02-28T06:36:40.360Z"
   },
   {
    "duration": 224,
    "start_time": "2022-02-28T06:36:40.418Z"
   },
   {
    "duration": 1170,
    "start_time": "2022-02-28T06:36:40.645Z"
   },
   {
    "duration": 1155,
    "start_time": "2022-02-28T06:36:41.817Z"
   },
   {
    "duration": 72693,
    "start_time": "2022-02-28T06:36:42.974Z"
   },
   {
    "duration": 65449,
    "start_time": "2022-02-28T06:37:55.669Z"
   },
   {
    "duration": 30900,
    "start_time": "2022-02-28T06:39:01.120Z"
   },
   {
    "duration": 1440,
    "start_time": "2022-02-28T06:39:32.022Z"
   },
   {
    "duration": 7598,
    "start_time": "2022-02-28T06:39:33.464Z"
   },
   {
    "duration": 447,
    "start_time": "2022-02-28T06:39:41.066Z"
   },
   {
    "duration": 146611,
    "start_time": "2022-02-28T06:39:50.016Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-28T06:55:33.903Z"
   },
   {
    "duration": 1351,
    "start_time": "2022-02-28T07:02:45.744Z"
   },
   {
    "duration": 1176,
    "start_time": "2022-02-28T07:02:59.685Z"
   },
   {
    "duration": 48,
    "start_time": "2022-02-28T07:03:00.863Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-28T07:03:00.913Z"
   },
   {
    "duration": 58,
    "start_time": "2022-02-28T07:03:00.926Z"
   },
   {
    "duration": 15,
    "start_time": "2022-02-28T07:03:00.986Z"
   },
   {
    "duration": 98,
    "start_time": "2022-02-28T07:03:01.003Z"
   },
   {
    "duration": 99,
    "start_time": "2022-02-28T07:03:01.104Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-28T07:03:01.205Z"
   },
   {
    "duration": 15,
    "start_time": "2022-02-28T07:03:01.227Z"
   },
   {
    "duration": 221,
    "start_time": "2022-02-28T07:03:01.244Z"
   },
   {
    "duration": 68,
    "start_time": "2022-02-28T07:03:01.467Z"
   },
   {
    "duration": 136,
    "start_time": "2022-02-28T07:03:01.603Z"
   },
   {
    "duration": 843,
    "start_time": "2022-02-28T07:03:01.741Z"
   },
   {
    "duration": 116,
    "start_time": "2022-02-28T07:03:02.586Z"
   },
   {
    "duration": 143,
    "start_time": "2022-02-28T07:03:02.705Z"
   },
   {
    "duration": 1131,
    "start_time": "2022-02-28T07:03:02.850Z"
   },
   {
    "duration": 1139,
    "start_time": "2022-02-28T07:03:03.983Z"
   },
   {
    "duration": 70523,
    "start_time": "2022-02-28T07:03:05.124Z"
   },
   {
    "duration": 65365,
    "start_time": "2022-02-28T07:04:15.649Z"
   },
   {
    "duration": 32284,
    "start_time": "2022-02-28T07:05:21.017Z"
   },
   {
    "duration": 1481,
    "start_time": "2022-02-28T07:05:53.303Z"
   },
   {
    "duration": 8524,
    "start_time": "2022-02-28T07:05:54.786Z"
   },
   {
    "duration": 455,
    "start_time": "2022-02-28T07:06:03.313Z"
   },
   {
    "duration": 1082,
    "start_time": "2022-02-28T07:06:10.547Z"
   },
   {
    "duration": 687138,
    "start_time": "2022-02-28T07:06:39.972Z"
   },
   {
    "duration": 12965,
    "start_time": "2022-02-28T07:19:31.137Z"
   },
   {
    "duration": 8261,
    "start_time": "2022-02-28T07:20:27.585Z"
   },
   {
    "duration": 26547,
    "start_time": "2022-02-28T07:27:16.576Z"
   },
   {
    "duration": 26131,
    "start_time": "2022-02-28T07:32:41.535Z"
   },
   {
    "duration": 321,
    "start_time": "2022-02-28T08:13:16.443Z"
   },
   {
    "duration": 27227,
    "start_time": "2022-02-28T08:13:43.627Z"
   },
   {
    "duration": 18426,
    "start_time": "2022-02-28T08:14:49.819Z"
   },
   {
    "duration": 26747,
    "start_time": "2022-02-28T08:16:12.954Z"
   },
   {
    "duration": 27117,
    "start_time": "2022-02-28T08:21:57.050Z"
   },
   {
    "duration": 77,
    "start_time": "2022-02-28T08:23:30.459Z"
   },
   {
    "duration": 84,
    "start_time": "2022-02-28T08:24:08.729Z"
   },
   {
    "duration": 108,
    "start_time": "2022-02-28T08:24:16.441Z"
   },
   {
    "duration": 15851,
    "start_time": "2022-02-28T08:26:58.218Z"
   },
   {
    "duration": 15362,
    "start_time": "2022-02-28T08:27:45.482Z"
   },
   {
    "duration": 8395,
    "start_time": "2022-02-28T08:29:07.178Z"
   },
   {
    "duration": 109073,
    "start_time": "2022-02-28T08:29:19.914Z"
   },
   {
    "duration": 70,
    "start_time": "2022-02-28T08:36:04.137Z"
   },
   {
    "duration": 13710,
    "start_time": "2022-02-28T08:36:15.496Z"
   },
   {
    "duration": 677,
    "start_time": "2022-02-28T08:37:21.625Z"
   },
   {
    "duration": 13413,
    "start_time": "2022-02-28T08:38:11.799Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-28T08:38:36.264Z"
   },
   {
    "duration": 89,
    "start_time": "2022-02-28T08:39:52.299Z"
   },
   {
    "duration": 14173,
    "start_time": "2022-02-28T08:40:06.568Z"
   },
   {
    "duration": 29757,
    "start_time": "2022-02-28T08:40:35.786Z"
   },
   {
    "duration": 14070,
    "start_time": "2022-02-28T08:41:30.105Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-28T08:42:20.057Z"
   },
   {
    "duration": 610,
    "start_time": "2022-02-28T08:43:47.064Z"
   },
   {
    "duration": 458,
    "start_time": "2022-02-28T08:43:55.751Z"
   },
   {
    "duration": 445,
    "start_time": "2022-02-28T08:44:01.113Z"
   },
   {
    "duration": 247,
    "start_time": "2022-02-28T08:46:24.424Z"
   },
   {
    "duration": 24648,
    "start_time": "2022-02-28T08:52:57.590Z"
   },
   {
    "duration": 50053,
    "start_time": "2022-02-28T08:54:02.312Z"
   },
   {
    "duration": 48166,
    "start_time": "2022-02-28T08:55:23.717Z"
   },
   {
    "duration": 20,
    "start_time": "2022-02-28T08:56:11.885Z"
   },
   {
    "duration": 13,
    "start_time": "2022-02-28T08:56:35.093Z"
   },
   {
    "duration": 176,
    "start_time": "2022-02-28T08:56:36.309Z"
   },
   {
    "duration": 179,
    "start_time": "2022-02-28T08:56:58.053Z"
   },
   {
    "duration": 96,
    "start_time": "2022-02-28T09:01:09.125Z"
   },
   {
    "duration": 455,
    "start_time": "2022-02-28T09:01:15.047Z"
   },
   {
    "duration": 335,
    "start_time": "2022-02-28T09:02:17.333Z"
   },
   {
    "duration": 216,
    "start_time": "2022-02-28T09:02:26.020Z"
   },
   {
    "duration": 604,
    "start_time": "2022-02-28T09:02:38.916Z"
   },
   {
    "duration": 667,
    "start_time": "2022-02-28T09:02:43.365Z"
   },
   {
    "duration": 288,
    "start_time": "2022-02-28T09:03:06.709Z"
   },
   {
    "duration": 452,
    "start_time": "2022-02-28T09:03:30.420Z"
   },
   {
    "duration": 107933,
    "start_time": "2022-02-28T09:03:42.469Z"
   },
   {
    "duration": 488,
    "start_time": "2022-02-28T09:06:30.820Z"
   },
   {
    "duration": 461,
    "start_time": "2022-02-28T09:06:45.395Z"
   },
   {
    "duration": 782,
    "start_time": "2022-02-28T09:08:30.612Z"
   },
   {
    "duration": 636,
    "start_time": "2022-02-28T09:08:36.291Z"
   },
   {
    "duration": 484,
    "start_time": "2022-02-28T09:08:41.555Z"
   },
   {
    "duration": 493,
    "start_time": "2022-02-28T09:08:46.851Z"
   },
   {
    "duration": 287,
    "start_time": "2022-02-28T09:10:24.467Z"
   },
   {
    "duration": 447,
    "start_time": "2022-02-28T09:10:43.987Z"
   },
   {
    "duration": 335,
    "start_time": "2022-02-28T09:11:21.107Z"
   },
   {
    "duration": 714,
    "start_time": "2022-02-28T09:11:26.531Z"
   },
   {
    "duration": 226,
    "start_time": "2022-02-28T09:11:31.891Z"
   },
   {
    "duration": 506,
    "start_time": "2022-02-28T09:11:40.563Z"
   },
   {
    "duration": 1226,
    "start_time": "2022-02-28T09:12:18.932Z"
   },
   {
    "duration": 51,
    "start_time": "2022-02-28T09:12:20.160Z"
   },
   {
    "duration": 12,
    "start_time": "2022-02-28T09:12:20.213Z"
   },
   {
    "duration": 33,
    "start_time": "2022-02-28T09:12:20.227Z"
   },
   {
    "duration": 41,
    "start_time": "2022-02-28T09:12:20.262Z"
   },
   {
    "duration": 100,
    "start_time": "2022-02-28T09:12:20.305Z"
   },
   {
    "duration": 96,
    "start_time": "2022-02-28T09:12:20.407Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-28T09:12:20.507Z"
   },
   {
    "duration": 9,
    "start_time": "2022-02-28T09:12:20.516Z"
   },
   {
    "duration": 242,
    "start_time": "2022-02-28T09:12:20.527Z"
   },
   {
    "duration": 134,
    "start_time": "2022-02-28T09:12:20.771Z"
   },
   {
    "duration": 131,
    "start_time": "2022-02-28T09:12:20.907Z"
   },
   {
    "duration": 810,
    "start_time": "2022-02-28T09:12:21.040Z"
   },
   {
    "duration": 68,
    "start_time": "2022-02-28T09:12:21.852Z"
   },
   {
    "duration": 220,
    "start_time": "2022-02-28T09:12:21.922Z"
   },
   {
    "duration": 1318,
    "start_time": "2022-02-28T09:12:22.145Z"
   },
   {
    "duration": 1279,
    "start_time": "2022-02-28T09:12:23.465Z"
   },
   {
    "duration": 79995,
    "start_time": "2022-02-28T09:12:24.746Z"
   },
   {
    "duration": 72208,
    "start_time": "2022-02-28T09:13:44.743Z"
   },
   {
    "duration": 34187,
    "start_time": "2022-02-28T09:14:56.952Z"
   },
   {
    "duration": 1574,
    "start_time": "2022-02-28T09:15:31.141Z"
   },
   {
    "duration": 7936,
    "start_time": "2022-02-28T09:15:32.717Z"
   },
   {
    "duration": 458,
    "start_time": "2022-02-28T09:15:40.657Z"
   },
   {
    "duration": 27632,
    "start_time": "2022-02-28T09:15:41.117Z"
   },
   {
    "duration": 120114,
    "start_time": "2022-02-28T09:16:08.751Z"
   },
   {
    "duration": 14593,
    "start_time": "2022-02-28T09:18:08.867Z"
   },
   {
    "duration": 47939,
    "start_time": "2022-02-28T09:18:23.462Z"
   },
   {
    "duration": 98,
    "start_time": "2022-02-28T09:19:11.403Z"
   },
   {
    "duration": 144,
    "start_time": "2022-02-28T09:19:11.504Z"
   },
   {
    "duration": 61,
    "start_time": "2022-02-28T09:19:11.650Z"
   },
   {
    "duration": 11,
    "start_time": "2022-02-28T09:19:11.713Z"
   },
   {
    "duration": 206,
    "start_time": "2022-02-28T09:19:11.725Z"
   },
   {
    "duration": 1104,
    "start_time": "2022-02-28T13:06:32.412Z"
   },
   {
    "duration": 47,
    "start_time": "2022-02-28T13:06:33.519Z"
   },
   {
    "duration": 10,
    "start_time": "2022-02-28T13:08:34.714Z"
   },
   {
    "duration": 19,
    "start_time": "2022-02-28T13:10:06.925Z"
   },
   {
    "duration": 13,
    "start_time": "2022-02-28T13:10:07.387Z"
   },
   {
    "duration": 17,
    "start_time": "2022-02-28T13:10:08.451Z"
   },
   {
    "duration": 5,
    "start_time": "2022-02-28T13:10:08.917Z"
   },
   {
    "duration": 6,
    "start_time": "2022-02-28T13:10:09.859Z"
   },
   {
    "duration": 4,
    "start_time": "2022-02-28T13:10:10.254Z"
   },
   {
    "duration": 174,
    "start_time": "2022-02-28T13:10:10.584Z"
   },
   {
    "duration": 52,
    "start_time": "2022-02-28T13:15:17.847Z"
   },
   {
    "duration": 36,
    "start_time": "2022-02-28T13:15:18.998Z"
   },
   {
    "duration": 656,
    "start_time": "2022-02-28T13:15:19.622Z"
   },
   {
    "duration": 39,
    "start_time": "2022-02-28T13:15:42.129Z"
   },
   {
    "duration": 47,
    "start_time": "2022-02-28T13:16:06.984Z"
   },
   {
    "duration": 951,
    "start_time": "2022-02-28T13:16:07.669Z"
   },
   {
    "duration": 961,
    "start_time": "2022-02-28T13:16:11.342Z"
   },
   {
    "duration": 60855,
    "start_time": "2022-02-28T13:16:17.448Z"
   },
   {
    "duration": 68199,
    "start_time": "2022-02-28T13:17:18.304Z"
   },
   {
    "duration": 27190,
    "start_time": "2022-02-28T13:18:26.506Z"
   },
   {
    "duration": 1321,
    "start_time": "2022-02-28T13:18:53.697Z"
   },
   {
    "duration": 6338,
    "start_time": "2022-02-28T13:18:55.019Z"
   },
   {
    "duration": 380,
    "start_time": "2022-02-28T13:19:01.358Z"
   },
   {
    "duration": 23216,
    "start_time": "2022-02-28T13:19:01.740Z"
   },
   {
    "duration": 92624,
    "start_time": "2022-02-28T13:19:24.958Z"
   },
   {
    "duration": 11616,
    "start_time": "2022-02-28T13:20:57.584Z"
   },
   {
    "duration": 36411,
    "start_time": "2022-02-28T13:21:09.202Z"
   },
   {
    "duration": 89,
    "start_time": "2022-02-28T13:21:45.615Z"
   },
   {
    "duration": 123,
    "start_time": "2022-02-28T13:21:45.709Z"
   },
   {
    "duration": 37,
    "start_time": "2022-02-28T13:21:45.834Z"
   },
   {
    "duration": 30,
    "start_time": "2022-02-28T13:21:45.872Z"
   },
   {
    "duration": 1104,
    "start_time": "2022-03-01T06:40:55.398Z"
   },
   {
    "duration": 52,
    "start_time": "2022-03-01T06:40:56.503Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-01T06:40:56.557Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-01T06:40:56.567Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-01T06:40:56.585Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-01T06:40:56.598Z"
   },
   {
    "duration": 90,
    "start_time": "2022-03-01T06:40:56.619Z"
   },
   {
    "duration": 103,
    "start_time": "2022-03-01T06:40:56.712Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-01T06:40:56.817Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-01T06:40:56.823Z"
   },
   {
    "duration": 98,
    "start_time": "2022-03-01T06:40:57.009Z"
   },
   {
    "duration": 127,
    "start_time": "2022-03-01T06:40:57.109Z"
   },
   {
    "duration": 651,
    "start_time": "2022-03-01T06:40:57.237Z"
   },
   {
    "duration": 42,
    "start_time": "2022-03-01T06:40:57.890Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-01T06:46:36.569Z"
   },
   {
    "duration": 1089,
    "start_time": "2022-03-01T15:34:55.268Z"
   },
   {
    "duration": 65,
    "start_time": "2022-03-01T15:34:56.359Z"
   },
   {
    "duration": 10,
    "start_time": "2022-03-01T15:34:56.425Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-01T15:34:57.488Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-01T15:34:57.509Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-01T15:34:58.009Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-01T15:34:58.746Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-01T15:35:00.074Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-01T15:35:01.588Z"
   },
   {
    "duration": 195,
    "start_time": "2022-03-01T15:35:02.904Z"
   },
   {
    "duration": 89,
    "start_time": "2022-03-01T15:35:06.554Z"
   },
   {
    "duration": 38,
    "start_time": "2022-03-01T15:35:06.964Z"
   },
   {
    "duration": 720,
    "start_time": "2022-03-01T15:35:07.168Z"
   },
   {
    "duration": 45,
    "start_time": "2022-03-01T15:35:07.929Z"
   },
   {
    "duration": 53,
    "start_time": "2022-03-01T15:35:09.391Z"
   },
   {
    "duration": 1029,
    "start_time": "2022-03-01T15:35:09.846Z"
   },
   {
    "duration": 1038,
    "start_time": "2022-03-01T15:35:10.877Z"
   },
   {
    "duration": 63869,
    "start_time": "2022-03-01T15:35:11.917Z"
   },
   {
    "duration": 58669,
    "start_time": "2022-03-01T15:36:15.788Z"
   },
   {
    "duration": 28279,
    "start_time": "2022-03-01T15:37:14.458Z"
   },
   {
    "duration": 1267,
    "start_time": "2022-03-01T15:37:42.738Z"
   },
   {
    "duration": 6594,
    "start_time": "2022-03-01T15:37:44.006Z"
   },
   {
    "duration": 406,
    "start_time": "2022-03-01T15:37:50.603Z"
   },
   {
    "duration": 24027,
    "start_time": "2022-03-01T15:37:51.011Z"
   },
   {
    "duration": 98027,
    "start_time": "2022-03-01T15:38:15.040Z"
   },
   {
    "duration": 12654,
    "start_time": "2022-03-01T15:39:53.069Z"
   },
   {
    "duration": 39248,
    "start_time": "2022-03-01T15:40:05.732Z"
   },
   {
    "duration": 160,
    "start_time": "2022-03-01T15:40:44.982Z"
   },
   {
    "duration": 125,
    "start_time": "2022-03-01T15:40:45.144Z"
   },
   {
    "duration": 40,
    "start_time": "2022-03-01T15:40:45.271Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-01T15:40:45.313Z"
   },
   {
    "duration": 279,
    "start_time": "2022-03-01T15:40:45.346Z"
   },
   {
    "duration": 40014,
    "start_time": "2022-03-01T15:59:37.534Z"
   },
   {
    "duration": 39905,
    "start_time": "2022-03-01T16:00:58.404Z"
   },
   {
    "duration": 10,
    "start_time": "2022-03-01T16:06:55.120Z"
   },
   {
    "duration": 35,
    "start_time": "2022-03-01T16:08:13.152Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-01T16:08:14.110Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-01T16:08:16.573Z"
   },
   {
    "duration": 13,
    "start_time": "2022-03-01T16:08:16.863Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-01T16:08:17.330Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-01T16:08:18.146Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-01T16:08:18.659Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-01T16:08:18.975Z"
   },
   {
    "duration": 186,
    "start_time": "2022-03-01T16:08:19.435Z"
   },
   {
    "duration": 40,
    "start_time": "2022-03-01T16:08:20.346Z"
   },
   {
    "duration": 44,
    "start_time": "2022-03-01T16:08:21.100Z"
   },
   {
    "duration": 630,
    "start_time": "2022-03-01T16:08:21.283Z"
   },
   {
    "duration": 48,
    "start_time": "2022-03-01T16:08:21.914Z"
   },
   {
    "duration": 42,
    "start_time": "2022-03-01T16:08:22.254Z"
   },
   {
    "duration": 946,
    "start_time": "2022-03-01T16:08:22.416Z"
   },
   {
    "duration": 944,
    "start_time": "2022-03-01T16:08:23.364Z"
   },
   {
    "duration": 58342,
    "start_time": "2022-03-01T16:08:27.987Z"
   },
   {
    "duration": 49327,
    "start_time": "2022-03-01T16:09:26.333Z"
   },
   {
    "duration": 21085,
    "start_time": "2022-03-01T16:10:15.662Z"
   },
   {
    "duration": 986,
    "start_time": "2022-03-01T16:10:36.750Z"
   },
   {
    "duration": 4865,
    "start_time": "2022-03-01T16:10:37.738Z"
   },
   {
    "duration": 356,
    "start_time": "2022-03-01T16:10:42.605Z"
   },
   {
    "duration": 22104,
    "start_time": "2022-03-01T16:10:42.962Z"
   },
   {
    "duration": 88590,
    "start_time": "2022-03-01T16:11:05.069Z"
   },
   {
    "duration": 16719,
    "start_time": "2022-03-01T16:12:33.661Z"
   },
   {
    "duration": 53871,
    "start_time": "2022-03-01T16:12:50.382Z"
   },
   {
    "duration": 85,
    "start_time": "2022-03-01T16:13:44.254Z"
   },
   {
    "duration": 122,
    "start_time": "2022-03-01T16:13:44.341Z"
   },
   {
    "duration": 30,
    "start_time": "2022-03-01T16:13:44.464Z"
   },
   {
    "duration": 9,
    "start_time": "2022-03-01T16:13:44.496Z"
   },
   {
    "duration": 1457,
    "start_time": "2022-03-01T17:32:13.765Z"
   },
   {
    "duration": 63,
    "start_time": "2022-03-01T17:32:15.224Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-01T17:32:15.289Z"
   },
   {
    "duration": 34,
    "start_time": "2022-03-01T17:32:15.311Z"
   },
   {
    "duration": 51,
    "start_time": "2022-03-01T17:32:15.347Z"
   },
   {
    "duration": 92,
    "start_time": "2022-03-01T17:32:15.400Z"
   },
   {
    "duration": 97,
    "start_time": "2022-03-01T17:32:15.495Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-01T17:32:15.594Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-01T17:32:15.605Z"
   },
   {
    "duration": 349,
    "start_time": "2022-03-01T17:32:15.612Z"
   },
   {
    "duration": 132,
    "start_time": "2022-03-01T17:32:15.964Z"
   },
   {
    "duration": 54,
    "start_time": "2022-03-01T17:32:16.188Z"
   },
   {
    "duration": 1056,
    "start_time": "2022-03-01T17:32:16.244Z"
   },
   {
    "duration": 88,
    "start_time": "2022-03-01T17:32:17.303Z"
   },
   {
    "duration": 217,
    "start_time": "2022-03-01T17:32:17.394Z"
   },
   {
    "duration": 1444,
    "start_time": "2022-03-01T17:32:17.614Z"
   },
   {
    "duration": 1542,
    "start_time": "2022-03-01T17:32:19.061Z"
   },
   {
    "duration": 88244,
    "start_time": "2022-03-01T17:32:20.606Z"
   },
   {
    "duration": 74250,
    "start_time": "2022-03-01T17:33:48.852Z"
   },
   {
    "duration": 32183,
    "start_time": "2022-03-01T17:35:03.104Z"
   },
   {
    "duration": 1439,
    "start_time": "2022-03-01T17:35:35.289Z"
   },
   {
    "duration": 7200,
    "start_time": "2022-03-01T17:35:36.731Z"
   },
   {
    "duration": 517,
    "start_time": "2022-03-01T17:35:43.934Z"
   },
   {
    "duration": 31950,
    "start_time": "2022-03-01T17:35:44.453Z"
   },
   {
    "duration": 137275,
    "start_time": "2022-03-01T17:36:16.405Z"
   },
   {
    "duration": 24870,
    "start_time": "2022-03-01T17:38:33.687Z"
   },
   {
    "duration": 80589,
    "start_time": "2022-03-01T17:38:58.562Z"
   },
   {
    "duration": 233,
    "start_time": "2022-03-01T17:40:19.154Z"
   },
   {
    "duration": 52,
    "start_time": "2022-03-01T17:40:19.391Z"
   },
   {
    "duration": 74,
    "start_time": "2022-03-01T17:40:19.446Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-01T17:40:19.522Z"
   },
   {
    "duration": 401,
    "start_time": "2022-03-01T17:40:19.538Z"
   },
   {
    "duration": 241,
    "start_time": "2022-03-01T17:48:01.809Z"
   },
   {
    "duration": 265,
    "start_time": "2022-03-01T17:48:17.441Z"
   },
   {
    "duration": 1606,
    "start_time": "2022-03-18T09:29:35.832Z"
   },
   {
    "duration": 54,
    "start_time": "2022-03-18T09:29:39.817Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-18T09:29:48.871Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-18T09:37:40.631Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-18T09:37:53.765Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-18T09:37:58.999Z"
   },
   {
    "duration": 32,
    "start_time": "2022-03-18T09:39:04.870Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T09:39:17.614Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T09:39:55.350Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T09:40:06.956Z"
   },
   {
    "duration": 130,
    "start_time": "2022-03-18T09:40:29.750Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-18T09:40:49.622Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-18T09:40:52.358Z"
   },
   {
    "duration": 633,
    "start_time": "2022-03-18T09:40:53.332Z"
   },
   {
    "duration": 78,
    "start_time": "2022-03-18T09:40:57.989Z"
   },
   {
    "duration": 39,
    "start_time": "2022-03-18T09:41:00.663Z"
   },
   {
    "duration": 869,
    "start_time": "2022-03-18T09:41:01.333Z"
   },
   {
    "duration": 845,
    "start_time": "2022-03-18T09:41:03.029Z"
   },
   {
    "duration": 52683,
    "start_time": "2022-03-18T09:41:11.046Z"
   },
   {
    "duration": 41855,
    "start_time": "2022-03-18T09:54:56.756Z"
   },
   {
    "duration": 39788,
    "start_time": "2022-03-18T09:55:52.020Z"
   },
   {
    "duration": 18453,
    "start_time": "2022-03-18T09:56:37.716Z"
   },
   {
    "duration": 795,
    "start_time": "2022-03-18T09:57:05.988Z"
   },
   {
    "duration": 4152,
    "start_time": "2022-03-18T09:57:23.492Z"
   },
   {
    "duration": 649,
    "start_time": "2022-03-18T09:57:43.316Z"
   },
   {
    "duration": 40453,
    "start_time": "2022-03-18T09:57:57.300Z"
   },
   {
    "duration": 81984,
    "start_time": "2022-03-18T09:58:54.772Z"
   },
   {
    "duration": 30602,
    "start_time": "2022-03-18T10:00:45.956Z"
   },
   {
    "duration": 106241,
    "start_time": "2022-03-18T10:01:21.124Z"
   },
   {
    "duration": 33,
    "start_time": "2022-03-18T10:03:30.852Z"
   },
   {
    "duration": 33,
    "start_time": "2022-03-18T10:03:32.452Z"
   },
   {
    "duration": 35,
    "start_time": "2022-03-18T10:03:38.819Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-18T10:03:40.404Z"
   },
   {
    "duration": 113,
    "start_time": "2022-03-18T10:04:11.219Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T10:04:30.257Z"
   },
   {
    "duration": 57,
    "start_time": "2022-03-18T10:04:30.263Z"
   },
   {
    "duration": 16,
    "start_time": "2022-03-18T10:04:30.321Z"
   },
   {
    "duration": 37,
    "start_time": "2022-03-18T10:04:30.339Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-18T10:04:30.378Z"
   },
   {
    "duration": 74,
    "start_time": "2022-03-18T10:04:30.398Z"
   },
   {
    "duration": 95,
    "start_time": "2022-03-18T10:04:30.475Z"
   },
   {
    "duration": 104,
    "start_time": "2022-03-18T10:04:30.573Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-18T10:04:30.679Z"
   },
   {
    "duration": 124,
    "start_time": "2022-03-18T10:04:30.708Z"
   },
   {
    "duration": 135,
    "start_time": "2022-03-18T10:04:30.834Z"
   },
   {
    "duration": 121,
    "start_time": "2022-03-18T10:04:30.971Z"
   },
   {
    "duration": 635,
    "start_time": "2022-03-18T10:04:31.094Z"
   },
   {
    "duration": 66,
    "start_time": "2022-03-18T10:04:31.730Z"
   },
   {
    "duration": 197,
    "start_time": "2022-03-18T10:04:31.798Z"
   },
   {
    "duration": 888,
    "start_time": "2022-03-18T10:04:31.996Z"
   },
   {
    "duration": 868,
    "start_time": "2022-03-18T10:04:32.886Z"
   },
   {
    "duration": 52756,
    "start_time": "2022-03-18T10:04:33.756Z"
   },
   {
    "duration": 41002,
    "start_time": "2022-03-18T10:05:26.514Z"
   },
   {
    "duration": 18272,
    "start_time": "2022-03-18T10:06:07.518Z"
   },
   {
    "duration": 797,
    "start_time": "2022-03-18T10:06:25.792Z"
   },
   {
    "duration": 4057,
    "start_time": "2022-03-18T10:06:26.591Z"
   },
   {
    "duration": 668,
    "start_time": "2022-03-18T10:06:30.649Z"
   },
   {
    "duration": 38954,
    "start_time": "2022-03-18T10:06:31.319Z"
   },
   {
    "duration": 79297,
    "start_time": "2022-03-18T10:07:10.275Z"
   },
   {
    "duration": 30134,
    "start_time": "2022-03-18T10:08:29.574Z"
   },
   {
    "duration": 104599,
    "start_time": "2022-03-18T10:08:59.710Z"
   },
   {
    "duration": 53,
    "start_time": "2022-03-18T10:10:44.312Z"
   },
   {
    "duration": 198,
    "start_time": "2022-03-18T10:10:44.366Z"
   },
   {
    "duration": 37,
    "start_time": "2022-03-18T10:10:44.566Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-18T10:10:44.604Z"
   },
   {
    "duration": 120,
    "start_time": "2022-03-18T10:10:44.626Z"
   },
   {
    "duration": 220,
    "start_time": "2022-03-18T10:32:43.762Z"
   },
   {
    "duration": 116,
    "start_time": "2022-03-18T10:32:52.003Z"
   },
   {
    "duration": 117,
    "start_time": "2022-03-18T10:33:37.923Z"
   },
   {
    "duration": 1471,
    "start_time": "2022-03-18T10:40:17.817Z"
   },
   {
    "duration": 47,
    "start_time": "2022-03-18T10:40:19.291Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-18T10:40:19.340Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-18T10:40:19.370Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-18T10:40:19.391Z"
   },
   {
    "duration": 67,
    "start_time": "2022-03-18T10:40:19.405Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T10:40:19.564Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-18T10:40:19.571Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-18T10:40:19.581Z"
   },
   {
    "duration": 154,
    "start_time": "2022-03-18T10:40:19.591Z"
   },
   {
    "duration": 38,
    "start_time": "2022-03-18T10:40:19.747Z"
   },
   {
    "duration": 124,
    "start_time": "2022-03-18T10:40:19.865Z"
   },
   {
    "duration": 612,
    "start_time": "2022-03-18T10:40:19.991Z"
   },
   {
    "duration": 63,
    "start_time": "2022-03-18T10:40:20.606Z"
   },
   {
    "duration": 53076,
    "start_time": "2022-03-18T10:40:20.671Z"
   },
   {
    "duration": 41073,
    "start_time": "2022-03-18T10:41:13.749Z"
   },
   {
    "duration": 18156,
    "start_time": "2022-03-18T10:41:54.824Z"
   },
   {
    "duration": 821,
    "start_time": "2022-03-18T10:42:12.981Z"
   },
   {
    "duration": 4285,
    "start_time": "2022-03-18T10:42:13.804Z"
   },
   {
    "duration": 852,
    "start_time": "2022-03-18T10:42:18.091Z"
   },
   {
    "duration": 39362,
    "start_time": "2022-03-18T10:42:18.945Z"
   },
   {
    "duration": 80270,
    "start_time": "2022-03-18T10:42:58.309Z"
   },
   {
    "duration": 30275,
    "start_time": "2022-03-18T10:44:18.581Z"
   },
   {
    "duration": 104297,
    "start_time": "2022-03-18T10:44:48.858Z"
   },
   {
    "duration": 35,
    "start_time": "2022-03-18T10:46:33.157Z"
   },
   {
    "duration": 122,
    "start_time": "2022-03-18T10:46:33.264Z"
   },
   {
    "duration": 35,
    "start_time": "2022-03-18T10:46:33.388Z"
   },
   {
    "duration": 11,
    "start_time": "2022-03-18T10:46:33.425Z"
   },
   {
    "duration": 136,
    "start_time": "2022-03-18T10:46:33.438Z"
   },
   {
    "duration": 49,
    "start_time": "2022-03-23T17:55:16.457Z"
   },
   {
    "duration": 1905,
    "start_time": "2022-03-23T17:55:33.222Z"
   },
   {
    "duration": 48,
    "start_time": "2022-03-23T17:55:35.128Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-23T17:55:35.177Z"
   },
   {
    "duration": 16,
    "start_time": "2022-03-23T17:55:35.196Z"
   },
   {
    "duration": 11,
    "start_time": "2022-03-23T17:55:35.213Z"
   },
   {
    "duration": 57,
    "start_time": "2022-03-23T17:55:35.226Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-23T17:55:35.285Z"
   },
   {
    "duration": 99,
    "start_time": "2022-03-23T17:55:35.292Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-23T17:55:35.393Z"
   },
   {
    "duration": 191,
    "start_time": "2022-03-23T17:55:35.403Z"
   },
   {
    "duration": 87,
    "start_time": "2022-03-23T17:55:35.595Z"
   },
   {
    "duration": 115,
    "start_time": "2022-03-23T17:55:35.684Z"
   },
   {
    "duration": 680,
    "start_time": "2022-03-23T17:55:35.801Z"
   },
   {
    "duration": 107,
    "start_time": "2022-03-23T17:55:36.482Z"
   },
   {
    "duration": 1514,
    "start_time": "2022-03-23T17:55:47.599Z"
   },
   {
    "duration": 50,
    "start_time": "2022-03-23T17:55:49.115Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-23T17:55:49.166Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-23T17:55:49.187Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-23T17:55:49.205Z"
   },
   {
    "duration": 168,
    "start_time": "2022-03-23T17:55:49.219Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-23T17:55:49.390Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-23T17:55:49.398Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-23T17:55:49.406Z"
   },
   {
    "duration": 230,
    "start_time": "2022-03-23T17:55:49.414Z"
   },
   {
    "duration": 48,
    "start_time": "2022-03-23T17:55:49.646Z"
   },
   {
    "duration": 204,
    "start_time": "2022-03-23T17:55:49.696Z"
   },
   {
    "duration": 688,
    "start_time": "2022-03-23T17:55:49.902Z"
   },
   {
    "duration": 90,
    "start_time": "2022-03-23T17:55:50.592Z"
   },
   {
    "duration": 50352,
    "start_time": "2022-03-23T17:55:50.684Z"
   },
   {
    "duration": 43882,
    "start_time": "2022-03-23T17:56:41.037Z"
   },
   {
    "duration": 19394,
    "start_time": "2022-03-23T17:57:24.921Z"
   },
   {
    "duration": 797,
    "start_time": "2022-03-23T17:57:44.316Z"
   },
   {
    "duration": 4066,
    "start_time": "2022-03-23T17:57:45.115Z"
   },
   {
    "duration": 708,
    "start_time": "2022-03-23T17:57:49.182Z"
   },
   {
    "duration": 38119,
    "start_time": "2022-03-23T17:57:49.892Z"
   },
   {
    "duration": 78594,
    "start_time": "2022-03-23T17:58:28.013Z"
   },
   {
    "duration": 31549,
    "start_time": "2022-03-23T17:59:46.608Z"
   },
   {
    "duration": 102848,
    "start_time": "2022-03-23T18:00:18.159Z"
   },
   {
    "duration": 172,
    "start_time": "2022-03-23T18:02:01.009Z"
   },
   {
    "duration": 32,
    "start_time": "2022-03-23T18:02:01.183Z"
   },
   {
    "duration": 35,
    "start_time": "2022-03-23T18:02:01.217Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-23T18:02:01.255Z"
   },
   {
    "duration": 123,
    "start_time": "2022-03-23T18:02:01.293Z"
   }
  ],
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.5"
  },
  "toc": {
   "base_numbering": 1,
   "nav_menu": {
    "height": "106px",
    "width": "257px"
   },
   "number_sections": true,
   "sideBar": true,
   "skip_h1_title": true,
   "title_cell": "Содержание",
   "title_sidebar": "Contents",
   "toc_cell": true,
   "toc_position": {},
   "toc_section_display": true,
   "toc_window_display": true
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
