{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Выбор локации для скважины"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Описание проекта #\n",
    "\n",
    "Нужно решить, какие скважины выбрать в регионе разработки.\n",
    "\n",
    "**Шаги для выбора локации обычно такие:**\n",
    "\n",
    "* В избранном регионе собирают характеристики для скважин: качество нефти и объём её запасов;\n",
    "* Строят модель для предсказания объёма запасов в новых скважинах;\n",
    "* Выбирают скважины с самыми высокими оценками значений;\n",
    "* Определяют регион с максимальной суммарной прибылью отобранных скважин.\n",
    "\n",
    "**Шаги по выполнению проекта**\n",
    "\n",
    "1. Загрузить и подготовьть данные. \n",
    "\n",
    "2. Обучить и проверьть модель для каждого региона.\n",
    "\n",
    "3. Подготовьть данные для расчета прибыли.\n",
    "\n",
    "4. Напишите функцию для расчёта прибыли по выбранным скважинам и предсказаниям модели:\n",
    "    \n",
    "5. Посчитайте риски и прибыль для каждого региона:\n",
    " \n",
    "**Описание данных**\n",
    "\n",
    "* id — уникальный идентификатор скважины;\n",
    "* f0, f1, f2 — три признака точек (неважно, что они означают, но сами признаки значимы);\n",
    "* product — объём запасов в скважине (тыс. баррелей).\n",
    "\n",
    "**Условия задачи:**\n",
    "1. Для обучения модели подходит только линейная регрессия (остальные — недостаточно предсказуемые).\n",
    "2. При разведке региона исследуют 500 точек, из которых с помощью машинного обучения выбирают 200 лучших для разработки.\n",
    "3. Бюджет на разработку скважин в регионе — 10 млрд рублей.\n",
    "4. При нынешних ценах один баррель сырья приносит 450 рублей дохода. Доход с каждой единицы продукта составляет 450 тыс. рублей, поскольку объём указан в тысячах баррелей.\n",
    "5. После оценки рисков нужно оставить лишь те регионы, в которых вероятность убытков меньше 2.5%. Среди них выбирают регион с наибольшей средней прибылью.\n",
    "\n",
    "*Данные синтетические: детали контрактов и характеристики месторождений не разглашаются.*"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Вывод\n",
    "\n",
    "После всех расчетов можем рекомендовать к разработке только второй регион, так как он проходит порог риска убытков в 2,5 % с уровнем 1,7%. Средняя прибыль самая высокая по всем регионам и  равна 433,96 млн. руб. 95 % доверительный интервал находится на уровне: 42.39 млн. руб - 840.91 млн. руб."
   ]
  }
 ],
 "metadata": {
  "ExecuteTimeLog": [
   {
    "duration": 726,
    "start_time": "2022-03-10T10:47:39.461Z"
   },
   {
    "duration": 461,
    "start_time": "2022-03-10T10:48:51.619Z"
   },
   {
    "duration": 90,
    "start_time": "2022-03-10T10:50:31.127Z"
   },
   {
    "duration": 40,
    "start_time": "2022-03-10T10:50:43.700Z"
   },
   {
    "duration": 700,
    "start_time": "2022-03-10T11:07:17.186Z"
   },
   {
    "duration": 121,
    "start_time": "2022-03-10T11:45:13.390Z"
   },
   {
    "duration": 132,
    "start_time": "2022-03-10T11:45:34.398Z"
   },
   {
    "duration": 88,
    "start_time": "2022-03-10T11:50:12.110Z"
   },
   {
    "duration": 188,
    "start_time": "2022-03-10T11:50:35.517Z"
   },
   {
    "duration": 183,
    "start_time": "2022-03-10T11:51:17.198Z"
   },
   {
    "duration": 180,
    "start_time": "2022-03-10T11:52:24.686Z"
   },
   {
    "duration": 314,
    "start_time": "2022-03-10T11:56:48.062Z"
   },
   {
    "duration": 81,
    "start_time": "2022-03-10T12:05:21.435Z"
   },
   {
    "duration": 400,
    "start_time": "2022-03-10T12:05:27.643Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-10T12:05:56.140Z"
   },
   {
    "duration": 269,
    "start_time": "2022-03-10T12:06:00.830Z"
   },
   {
    "duration": -183,
    "start_time": "2022-03-10T12:08:19.949Z"
   },
   {
    "duration": 1476,
    "start_time": "2022-03-10T13:37:50.255Z"
   },
   {
    "duration": 584,
    "start_time": "2022-03-10T13:37:51.733Z"
   },
   {
    "duration": 40,
    "start_time": "2022-03-10T13:37:52.320Z"
   },
   {
    "duration": 195,
    "start_time": "2022-03-10T13:37:52.362Z"
   },
   {
    "duration": 194,
    "start_time": "2022-03-10T13:37:52.559Z"
   },
   {
    "duration": 14831,
    "start_time": "2022-03-10T13:37:58.928Z"
   },
   {
    "duration": 2026459,
    "start_time": "2022-03-10T13:38:52.631Z"
   },
   {
    "duration": 55,
    "start_time": "2022-03-10T14:12:39.037Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-10T14:12:43.254Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-10T14:13:01.794Z"
   },
   {
    "duration": 1247,
    "start_time": "2022-03-10T18:26:23.980Z"
   },
   {
    "duration": 957,
    "start_time": "2022-03-10T18:26:25.229Z"
   },
   {
    "duration": 37,
    "start_time": "2022-03-10T18:26:26.189Z"
   },
   {
    "duration": 142,
    "start_time": "2022-03-10T18:26:26.227Z"
   },
   {
    "duration": 157,
    "start_time": "2022-03-10T18:26:26.371Z"
   },
   {
    "duration": 1149,
    "start_time": "2022-03-11T05:29:13.873Z"
   },
   {
    "duration": 356,
    "start_time": "2022-03-11T05:29:15.024Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T05:29:15.382Z"
   },
   {
    "duration": 112,
    "start_time": "2022-03-11T05:29:15.415Z"
   },
   {
    "duration": 111,
    "start_time": "2022-03-11T05:29:15.529Z"
   },
   {
    "duration": 191,
    "start_time": "2022-03-11T05:32:57.569Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-11T05:33:11.359Z"
   },
   {
    "duration": 703,
    "start_time": "2022-03-11T05:34:17.390Z"
   },
   {
    "duration": 724,
    "start_time": "2022-03-11T05:35:50.991Z"
   },
   {
    "duration": 623,
    "start_time": "2022-03-11T05:36:51.919Z"
   },
   {
    "duration": 575,
    "start_time": "2022-03-11T05:37:39.774Z"
   },
   {
    "duration": 636,
    "start_time": "2022-03-11T05:37:57.151Z"
   },
   {
    "duration": 651,
    "start_time": "2022-03-11T05:38:17.502Z"
   },
   {
    "duration": 649,
    "start_time": "2022-03-11T05:38:24.047Z"
   },
   {
    "duration": 410,
    "start_time": "2022-03-11T05:38:31.007Z"
   },
   {
    "duration": 337,
    "start_time": "2022-03-11T05:39:07.902Z"
   },
   {
    "duration": 348,
    "start_time": "2022-03-11T05:42:18.125Z"
   },
   {
    "duration": 334,
    "start_time": "2022-03-11T05:43:31.438Z"
   },
   {
    "duration": 347,
    "start_time": "2022-03-11T05:43:51.005Z"
   },
   {
    "duration": 285,
    "start_time": "2022-03-11T05:54:20.557Z"
   },
   {
    "duration": 752,
    "start_time": "2022-03-11T05:54:32.860Z"
   },
   {
    "duration": 576,
    "start_time": "2022-03-11T05:54:47.885Z"
   },
   {
    "duration": 629,
    "start_time": "2022-03-11T05:55:12.109Z"
   },
   {
    "duration": 333,
    "start_time": "2022-03-11T05:57:02.332Z"
   },
   {
    "duration": 332,
    "start_time": "2022-03-11T05:57:21.292Z"
   },
   {
    "duration": 410,
    "start_time": "2022-03-11T05:57:32.652Z"
   },
   {
    "duration": 359,
    "start_time": "2022-03-11T05:57:44.204Z"
   },
   {
    "duration": 337,
    "start_time": "2022-03-11T05:57:53.323Z"
   },
   {
    "duration": 334,
    "start_time": "2022-03-11T05:58:28.668Z"
   },
   {
    "duration": 322,
    "start_time": "2022-03-11T05:59:18.653Z"
   },
   {
    "duration": 343,
    "start_time": "2022-03-11T05:59:36.828Z"
   },
   {
    "duration": 715,
    "start_time": "2022-03-11T06:00:15.244Z"
   },
   {
    "duration": 976,
    "start_time": "2022-03-11T06:00:50.556Z"
   },
   {
    "duration": 1299,
    "start_time": "2022-03-11T06:08:14.443Z"
   },
   {
    "duration": 1212,
    "start_time": "2022-03-11T06:12:07.691Z"
   },
   {
    "duration": 1330,
    "start_time": "2022-03-11T07:02:37.654Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-11T07:15:59.347Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-11T07:16:38.676Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-11T07:17:00.323Z"
   },
   {
    "duration": 332,
    "start_time": "2022-03-11T07:17:58.979Z"
   },
   {
    "duration": 327,
    "start_time": "2022-03-11T07:18:32.437Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-11T07:20:16.452Z"
   },
   {
    "duration": 13,
    "start_time": "2022-03-11T07:20:27.796Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-11T07:22:02.883Z"
   },
   {
    "duration": 329,
    "start_time": "2022-03-11T07:22:50.051Z"
   },
   {
    "duration": 330,
    "start_time": "2022-03-11T07:23:53.139Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-11T07:24:09.811Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-11T07:24:45.379Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-11T07:25:12.563Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-11T07:26:49.358Z"
   },
   {
    "duration": 162,
    "start_time": "2022-03-11T08:39:21.546Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-11T08:39:31.818Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-11T08:39:41.066Z"
   },
   {
    "duration": 372,
    "start_time": "2022-03-11T08:39:54.393Z"
   },
   {
    "duration": 24,
    "start_time": "2022-03-11T08:40:03.664Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-11T08:40:18.249Z"
   },
   {
    "duration": 553,
    "start_time": "2022-03-11T08:40:34.329Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-11T08:40:46.180Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-11T08:40:57.481Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-11T08:42:12.633Z"
   },
   {
    "duration": 324,
    "start_time": "2022-03-11T08:42:50.569Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-11T08:43:07.961Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-11T08:44:05.353Z"
   },
   {
    "duration": 306,
    "start_time": "2022-03-11T08:45:55.098Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-11T08:46:00.044Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-11T08:46:02.074Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-11T08:46:45.257Z"
   },
   {
    "duration": 9,
    "start_time": "2022-03-11T08:52:21.431Z"
   },
   {
    "duration": 328,
    "start_time": "2022-03-11T08:57:08.744Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-11T08:57:49.864Z"
   },
   {
    "duration": 11,
    "start_time": "2022-03-11T08:58:00.007Z"
   },
   {
    "duration": 13,
    "start_time": "2022-03-11T08:58:05.575Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-11T08:58:11.927Z"
   },
   {
    "duration": 11,
    "start_time": "2022-03-11T09:02:42.343Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T09:05:10.253Z"
   },
   {
    "duration": 370,
    "start_time": "2022-03-11T09:05:10.257Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-11T09:05:10.629Z"
   },
   {
    "duration": 113,
    "start_time": "2022-03-11T09:05:10.651Z"
   },
   {
    "duration": 102,
    "start_time": "2022-03-11T09:05:10.766Z"
   },
   {
    "duration": 1334,
    "start_time": "2022-03-11T09:05:19.609Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T09:07:34.186Z"
   },
   {
    "duration": 322,
    "start_time": "2022-03-11T09:25:12.680Z"
   },
   {
    "duration": 349,
    "start_time": "2022-03-11T09:25:55.273Z"
   },
   {
    "duration": 7953,
    "start_time": "2022-03-11T09:26:25.033Z"
   },
   {
    "duration": 1019,
    "start_time": "2022-03-11T09:28:40.759Z"
   },
   {
    "duration": 991,
    "start_time": "2022-03-11T09:31:00.635Z"
   },
   {
    "duration": 8479,
    "start_time": "2022-03-11T09:32:18.120Z"
   },
   {
    "duration": 7894,
    "start_time": "2022-03-11T09:34:12.311Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:01:22.532Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T10:01:42.100Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:01:51.956Z"
   },
   {
    "duration": 23503,
    "start_time": "2022-03-11T10:02:23.972Z"
   },
   {
    "duration": 24774,
    "start_time": "2022-03-11T10:06:25.541Z"
   },
   {
    "duration": 25254,
    "start_time": "2022-03-11T10:09:46.892Z"
   },
   {
    "duration": 23732,
    "start_time": "2022-03-11T10:11:22.020Z"
   },
   {
    "duration": 25147,
    "start_time": "2022-03-11T10:14:37.764Z"
   },
   {
    "duration": 25588,
    "start_time": "2022-03-11T10:16:37.876Z"
   },
   {
    "duration": 111138,
    "start_time": "2022-03-11T10:19:26.755Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-11T10:23:26.418Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:24:14.946Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:25:33.010Z"
   },
   {
    "duration": 1599,
    "start_time": "2022-03-11T10:26:14.531Z"
   },
   {
    "duration": 301,
    "start_time": "2022-03-11T10:27:19.426Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:27:39.665Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:27:54.689Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:28:13.761Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T10:29:05.459Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:29:45.137Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:30:05.571Z"
   },
   {
    "duration": 293,
    "start_time": "2022-03-11T10:30:11.235Z"
   },
   {
    "duration": 1646,
    "start_time": "2022-03-11T10:30:33.140Z"
   },
   {
    "duration": 97189,
    "start_time": "2022-03-11T10:31:56.535Z"
   },
   {
    "duration": 132861,
    "start_time": "2022-03-11T10:35:15.120Z"
   },
   {
    "duration": 52322,
    "start_time": "2022-03-11T10:41:56.551Z"
   },
   {
    "duration": 7955,
    "start_time": "2022-03-11T10:43:33.334Z"
   },
   {
    "duration": 9842,
    "start_time": "2022-03-11T10:44:10.932Z"
   },
   {
    "duration": 8176,
    "start_time": "2022-03-11T10:44:47.876Z"
   },
   {
    "duration": 2882,
    "start_time": "2022-03-11T10:45:44.832Z"
   },
   {
    "duration": 101,
    "start_time": "2022-03-11T10:46:30.591Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:46:33.310Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T10:46:46.958Z"
   },
   {
    "duration": 2933,
    "start_time": "2022-03-11T10:47:46.572Z"
   },
   {
    "duration": 7932,
    "start_time": "2022-03-11T10:48:48.331Z"
   },
   {
    "duration": 106,
    "start_time": "2022-03-11T10:49:10.074Z"
   },
   {
    "duration": 2970,
    "start_time": "2022-03-11T10:49:58.825Z"
   },
   {
    "duration": 7845,
    "start_time": "2022-03-11T10:50:44.536Z"
   },
   {
    "duration": 3447,
    "start_time": "2022-03-11T10:53:50.181Z"
   },
   {
    "duration": 3732,
    "start_time": "2022-03-11T10:55:31.637Z"
   },
   {
    "duration": 3520,
    "start_time": "2022-03-11T10:56:30.307Z"
   },
   {
    "duration": 343,
    "start_time": "2022-03-11T10:57:47.761Z"
   },
   {
    "duration": 3628,
    "start_time": "2022-03-11T10:58:03.425Z"
   },
   {
    "duration": 7675,
    "start_time": "2022-03-11T10:58:14.048Z"
   },
   {
    "duration": 7819,
    "start_time": "2022-03-11T10:59:27.985Z"
   },
   {
    "duration": 7865,
    "start_time": "2022-03-11T11:02:25.966Z"
   },
   {
    "duration": 7938,
    "start_time": "2022-03-11T11:02:47.230Z"
   },
   {
    "duration": 966,
    "start_time": "2022-03-11T11:23:23.563Z"
   },
   {
    "duration": 969,
    "start_time": "2022-03-11T11:23:39.082Z"
   },
   {
    "duration": 1003,
    "start_time": "2022-03-11T11:23:48.618Z"
   },
   {
    "duration": 911,
    "start_time": "2022-03-11T11:24:10.138Z"
   },
   {
    "duration": 7683,
    "start_time": "2022-03-11T11:24:39.834Z"
   },
   {
    "duration": 8053,
    "start_time": "2022-03-11T11:25:08.809Z"
   },
   {
    "duration": 9,
    "start_time": "2022-03-11T11:25:48.698Z"
   },
   {
    "duration": 311,
    "start_time": "2022-03-11T11:28:47.673Z"
   },
   {
    "duration": 950,
    "start_time": "2022-03-11T11:29:08.121Z"
   },
   {
    "duration": 2615,
    "start_time": "2022-03-11T11:29:22.682Z"
   },
   {
    "duration": 2539,
    "start_time": "2022-03-11T11:31:05.994Z"
   },
   {
    "duration": 2647,
    "start_time": "2022-03-11T11:31:10.425Z"
   },
   {
    "duration": 2713,
    "start_time": "2022-03-11T11:31:27.583Z"
   },
   {
    "duration": 2714,
    "start_time": "2022-03-11T11:32:00.633Z"
   },
   {
    "duration": 2603,
    "start_time": "2022-03-11T11:32:10.781Z"
   },
   {
    "duration": 2696,
    "start_time": "2022-03-11T11:41:16.633Z"
   },
   {
    "duration": 2716,
    "start_time": "2022-03-11T11:41:36.201Z"
   },
   {
    "duration": 1696,
    "start_time": "2022-03-11T11:41:44.969Z"
   },
   {
    "duration": 2619,
    "start_time": "2022-03-11T11:42:31.353Z"
   },
   {
    "duration": 2678,
    "start_time": "2022-03-11T11:43:04.426Z"
   },
   {
    "duration": 1143,
    "start_time": "2022-03-11T11:44:27.897Z"
   },
   {
    "duration": 2693,
    "start_time": "2022-03-11T11:44:36.985Z"
   },
   {
    "duration": 2730,
    "start_time": "2022-03-11T11:45:04.843Z"
   },
   {
    "duration": 1014,
    "start_time": "2022-03-11T11:45:29.960Z"
   },
   {
    "duration": 2586,
    "start_time": "2022-03-11T11:45:37.801Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-11T11:49:18.760Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T11:50:23.835Z"
   },
   {
    "duration": 368,
    "start_time": "2022-03-11T11:50:34.940Z"
   },
   {
    "duration": 360,
    "start_time": "2022-03-11T11:50:51.432Z"
   },
   {
    "duration": 328,
    "start_time": "2022-03-11T11:52:13.321Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-11T11:52:25.547Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-11T11:53:52.427Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-11T11:54:20.905Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-11T12:02:10.380Z"
   },
   {
    "duration": 1073,
    "start_time": "2022-03-11T12:05:12.663Z"
   },
   {
    "duration": 359,
    "start_time": "2022-03-11T12:05:13.738Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-11T12:05:14.099Z"
   },
   {
    "duration": 109,
    "start_time": "2022-03-11T12:05:14.122Z"
   },
   {
    "duration": 108,
    "start_time": "2022-03-11T12:05:14.233Z"
   },
   {
    "duration": 1375,
    "start_time": "2022-03-11T12:05:14.342Z"
   },
   {
    "duration": 7974,
    "start_time": "2022-03-11T12:05:15.718Z"
   },
   {
    "duration": 2710,
    "start_time": "2022-03-11T12:05:23.694Z"
   },
   {
    "duration": 2659,
    "start_time": "2022-03-11T12:05:26.405Z"
   },
   {
    "duration": 2785,
    "start_time": "2022-03-11T12:05:29.065Z"
   },
   {
    "duration": 50,
    "start_time": "2022-03-11T12:05:31.852Z"
   },
   {
    "duration": 114,
    "start_time": "2022-03-11T12:05:31.904Z"
   },
   {
    "duration": 190,
    "start_time": "2022-03-11T12:05:32.021Z"
   },
   {
    "duration": 1168,
    "start_time": "2022-03-11T15:18:13.742Z"
   },
   {
    "duration": 418,
    "start_time": "2022-03-11T15:18:14.912Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T15:18:15.334Z"
   },
   {
    "duration": 177,
    "start_time": "2022-03-11T15:18:15.367Z"
   },
   {
    "duration": 143,
    "start_time": "2022-03-11T15:18:15.546Z"
   },
   {
    "duration": 1682,
    "start_time": "2022-03-11T15:18:15.691Z"
   },
   {
    "duration": 6051,
    "start_time": "2022-03-11T15:18:17.374Z"
   },
   {
    "duration": 2055,
    "start_time": "2022-03-11T15:18:23.427Z"
   },
   {
    "duration": 2034,
    "start_time": "2022-03-11T15:18:25.484Z"
   },
   {
    "duration": 2111,
    "start_time": "2022-03-11T15:18:27.521Z"
   },
   {
    "duration": 76,
    "start_time": "2022-03-11T15:18:29.634Z"
   },
   {
    "duration": 118,
    "start_time": "2022-03-11T15:18:29.713Z"
   },
   {
    "duration": 116,
    "start_time": "2022-03-11T15:18:29.903Z"
   },
   {
    "duration": 1619,
    "start_time": "2022-03-11T15:20:21.284Z"
   },
   {
    "duration": 516,
    "start_time": "2022-03-11T15:20:22.905Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-11T15:20:23.424Z"
   },
   {
    "duration": 149,
    "start_time": "2022-03-11T15:20:23.453Z"
   },
   {
    "duration": 132,
    "start_time": "2022-03-11T15:20:23.604Z"
   },
   {
    "duration": 1606,
    "start_time": "2022-03-11T15:20:23.738Z"
   },
   {
    "duration": 108,
    "start_time": "2022-03-11T15:20:29.698Z"
   },
   {
    "duration": 6116,
    "start_time": "2022-03-11T15:20:53.705Z"
   },
   {
    "duration": 2127,
    "start_time": "2022-03-11T15:20:59.823Z"
   },
   {
    "duration": 2453,
    "start_time": "2022-03-11T15:21:01.953Z"
   },
   {
    "duration": 1988,
    "start_time": "2022-03-11T15:21:04.409Z"
   },
   {
    "duration": 104,
    "start_time": "2022-03-11T15:21:06.399Z"
   },
   {
    "duration": 190,
    "start_time": "2022-03-11T15:21:06.511Z"
   },
   {
    "duration": 114,
    "start_time": "2022-03-11T15:21:06.704Z"
   },
   {
    "duration": 1167,
    "start_time": "2022-03-11T17:53:47.626Z"
   },
   {
    "duration": 406,
    "start_time": "2022-03-11T17:53:48.795Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-11T17:53:49.203Z"
   },
   {
    "duration": 145,
    "start_time": "2022-03-11T17:53:49.233Z"
   },
   {
    "duration": 149,
    "start_time": "2022-03-11T17:53:49.380Z"
   },
   {
    "duration": 1565,
    "start_time": "2022-03-11T17:53:49.530Z"
   },
   {
    "duration": 5944,
    "start_time": "2022-03-11T17:53:51.102Z"
   },
   {
    "duration": 2008,
    "start_time": "2022-03-11T17:53:57.048Z"
   },
   {
    "duration": 2291,
    "start_time": "2022-03-11T17:53:59.059Z"
   },
   {
    "duration": 2280,
    "start_time": "2022-03-11T17:54:01.353Z"
   },
   {
    "duration": 70,
    "start_time": "2022-03-11T17:54:03.635Z"
   },
   {
    "duration": 115,
    "start_time": "2022-03-11T17:54:03.707Z"
   },
   {
    "duration": 201,
    "start_time": "2022-03-11T17:54:03.824Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-11T17:58:46.476Z"
   },
   {
    "duration": 29,
    "start_time": "2022-03-11T17:59:24.173Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-11T18:00:47.833Z"
   },
   {
    "duration": 34,
    "start_time": "2022-03-11T18:00:51.188Z"
   },
   {
    "duration": 30,
    "start_time": "2022-03-11T18:01:59.961Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T18:02:40.034Z"
   },
   {
    "duration": 105,
    "start_time": "2022-03-11T18:04:34.911Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-11T18:04:42.658Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T18:04:54.506Z"
   },
   {
    "duration": 45,
    "start_time": "2022-03-11T18:05:01.058Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-11T18:05:33.450Z"
   },
   {
    "duration": 25,
    "start_time": "2022-03-11T18:05:39.826Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-11T18:05:42.145Z"
   },
   {
    "duration": 108,
    "start_time": "2022-03-11T18:06:01.002Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-11T18:06:09.041Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T18:06:12.417Z"
   },
   {
    "duration": 409,
    "start_time": "2022-03-11T18:06:27.497Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-11T18:06:33.025Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-11T18:08:03.608Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-11T18:08:28.360Z"
   },
   {
    "duration": 30,
    "start_time": "2022-03-11T18:08:50.231Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-11T18:15:45.889Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-11T18:19:42.860Z"
   },
   {
    "duration": 15,
    "start_time": "2022-03-11T18:19:48.621Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-11T18:21:35.291Z"
   },
   {
    "duration": 25,
    "start_time": "2022-03-11T18:21:35.747Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-11T18:21:36.187Z"
   },
   {
    "duration": 15,
    "start_time": "2022-03-11T18:21:38.315Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T18:43:12.133Z"
   },
   {
    "duration": 425,
    "start_time": "2022-03-11T18:43:12.138Z"
   },
   {
    "duration": 37,
    "start_time": "2022-03-11T18:43:12.566Z"
   },
   {
    "duration": 131,
    "start_time": "2022-03-11T18:43:12.605Z"
   },
   {
    "duration": 132,
    "start_time": "2022-03-11T18:43:12.738Z"
   },
   {
    "duration": 1469,
    "start_time": "2022-03-11T18:43:12.871Z"
   },
   {
    "duration": 5883,
    "start_time": "2022-03-11T18:43:14.342Z"
   },
   {
    "duration": 2315,
    "start_time": "2022-03-11T18:43:20.227Z"
   },
   {
    "duration": 1926,
    "start_time": "2022-03-11T18:43:22.545Z"
   },
   {
    "duration": 2234,
    "start_time": "2022-03-11T18:43:24.473Z"
   },
   {
    "duration": 93,
    "start_time": "2022-03-11T18:43:26.709Z"
   },
   {
    "duration": 121,
    "start_time": "2022-03-11T18:43:26.805Z"
   },
   {
    "duration": 188,
    "start_time": "2022-03-11T18:43:26.929Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-11T18:43:27.119Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-11T18:43:27.306Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T18:43:56.690Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-11T18:52:39.219Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-11T18:52:45.901Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-11T18:53:19.462Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-11T18:54:59.492Z"
   },
   {
    "duration": 125,
    "start_time": "2022-03-11T19:01:04.951Z"
   },
   {
    "duration": 1217,
    "start_time": "2022-03-14T04:51:29.842Z"
   },
   {
    "duration": 409,
    "start_time": "2022-03-14T04:51:31.062Z"
   },
   {
    "duration": 38,
    "start_time": "2022-03-14T04:51:31.474Z"
   },
   {
    "duration": 139,
    "start_time": "2022-03-14T04:51:31.514Z"
   },
   {
    "duration": 148,
    "start_time": "2022-03-14T04:51:31.654Z"
   },
   {
    "duration": 1530,
    "start_time": "2022-03-14T04:51:31.805Z"
   },
   {
    "duration": 5921,
    "start_time": "2022-03-14T04:51:33.337Z"
   },
   {
    "duration": 2028,
    "start_time": "2022-03-14T04:51:39.261Z"
   },
   {
    "duration": 2021,
    "start_time": "2022-03-14T04:51:41.291Z"
   },
   {
    "duration": 2029,
    "start_time": "2022-03-14T04:51:43.313Z"
   },
   {
    "duration": 64,
    "start_time": "2022-03-14T04:51:45.344Z"
   },
   {
    "duration": 106,
    "start_time": "2022-03-14T04:51:45.410Z"
   },
   {
    "duration": 197,
    "start_time": "2022-03-14T04:51:45.518Z"
   },
   {
    "duration": 186,
    "start_time": "2022-03-14T04:51:45.718Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-14T04:51:45.907Z"
   },
   {
    "duration": 147,
    "start_time": "2022-03-14T04:51:45.913Z"
   },
   {
    "duration": -140,
    "start_time": "2022-03-14T05:22:11.023Z"
   },
   {
    "duration": 3152,
    "start_time": "2022-03-14T05:22:30.620Z"
   },
   {
    "duration": 260,
    "start_time": "2022-03-14T05:23:17.611Z"
   },
   {
    "duration": 1230,
    "start_time": "2022-03-14T05:25:43.764Z"
   },
   {
    "duration": 416,
    "start_time": "2022-03-14T05:25:44.997Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-14T05:25:45.415Z"
   },
   {
    "duration": 138,
    "start_time": "2022-03-14T05:25:45.444Z"
   },
   {
    "duration": 150,
    "start_time": "2022-03-14T05:25:45.583Z"
   },
   {
    "duration": 1660,
    "start_time": "2022-03-14T05:25:45.735Z"
   },
   {
    "duration": 6531,
    "start_time": "2022-03-14T05:25:47.401Z"
   },
   {
    "duration": 2061,
    "start_time": "2022-03-14T05:25:53.935Z"
   },
   {
    "duration": 2147,
    "start_time": "2022-03-14T05:25:55.998Z"
   },
   {
    "duration": 2343,
    "start_time": "2022-03-14T05:25:58.147Z"
   },
   {
    "duration": 33,
    "start_time": "2022-03-14T05:26:00.493Z"
   },
   {
    "duration": 205,
    "start_time": "2022-03-14T05:26:00.528Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-14T05:26:00.736Z"
   },
   {
    "duration": 90,
    "start_time": "2022-03-14T05:26:00.924Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-14T05:26:01.101Z"
   },
   {
    "duration": 128,
    "start_time": "2022-03-14T05:26:01.127Z"
   },
   {
    "duration": -140,
    "start_time": "2022-03-14T05:32:59.685Z"
   },
   {
    "duration": 294,
    "start_time": "2022-03-14T05:33:01.702Z"
   },
   {
    "duration": 278,
    "start_time": "2022-03-14T05:34:21.851Z"
   },
   {
    "duration": 78,
    "start_time": "2022-03-14T05:36:00.154Z"
   },
   {
    "duration": 83,
    "start_time": "2022-03-14T05:36:06.746Z"
   },
   {
    "duration": 305,
    "start_time": "2022-03-14T05:36:11.403Z"
   },
   {
    "duration": 307,
    "start_time": "2022-03-14T05:36:36.570Z"
   },
   {
    "duration": 339,
    "start_time": "2022-03-14T05:36:55.819Z"
   },
   {
    "duration": 1392,
    "start_time": "2022-03-14T05:37:45.962Z"
   },
   {
    "duration": 1361,
    "start_time": "2022-03-14T05:43:47.354Z"
   },
   {
    "duration": 600,
    "start_time": "2022-03-14T05:44:18.133Z"
   },
   {
    "duration": 80,
    "start_time": "2022-03-14T05:48:52.665Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-14T05:49:04.905Z"
   },
   {
    "duration": 9,
    "start_time": "2022-03-14T06:01:14.024Z"
   },
   {
    "duration": 415,
    "start_time": "2022-03-14T06:27:00.437Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-14T06:31:07.844Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-14T07:20:25.727Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-14T07:30:56.030Z"
   },
   {
    "duration": 11,
    "start_time": "2022-03-14T07:31:17.615Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-14T07:37:55.453Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-14T07:38:11.069Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-14T07:38:24.493Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-14T07:38:49.885Z"
   },
   {
    "duration": 320,
    "start_time": "2022-03-14T10:51:26.715Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-14T10:51:53.387Z"
   },
   {
    "duration": 258,
    "start_time": "2022-03-14T10:51:59.146Z"
   },
   {
    "duration": 258,
    "start_time": "2022-03-14T10:53:28.141Z"
   },
   {
    "duration": 276,
    "start_time": "2022-03-14T11:00:58.122Z"
   },
   {
    "duration": 804,
    "start_time": "2022-03-14T11:05:34.809Z"
   },
   {
    "duration": 1041,
    "start_time": "2022-03-14T11:11:17.512Z"
   },
   {
    "duration": 795,
    "start_time": "2022-03-14T11:11:35.449Z"
   },
   {
    "duration": 281,
    "start_time": "2022-03-14T11:14:18.184Z"
   },
   {
    "duration": 1356,
    "start_time": "2022-03-14T11:14:44.747Z"
   },
   {
    "duration": 1052,
    "start_time": "2022-03-14T11:14:54.024Z"
   },
   {
    "duration": 1006,
    "start_time": "2022-03-14T11:14:59.272Z"
   },
   {
    "duration": 1378,
    "start_time": "2022-03-14T11:16:00.025Z"
   },
   {
    "duration": 1103,
    "start_time": "2022-03-14T11:16:09.864Z"
   },
   {
    "duration": 1121,
    "start_time": "2022-03-14T11:16:44.014Z"
   },
   {
    "duration": 1382,
    "start_time": "2022-03-14T11:16:59.656Z"
   },
   {
    "duration": 967,
    "start_time": "2022-03-14T11:17:07.563Z"
   },
   {
    "duration": 1098,
    "start_time": "2022-03-14T11:17:16.376Z"
   },
   {
    "duration": 1038,
    "start_time": "2022-03-14T11:17:22.840Z"
   },
   {
    "duration": 1007,
    "start_time": "2022-03-14T11:18:13.646Z"
   },
   {
    "duration": 1072,
    "start_time": "2022-03-14T11:20:37.083Z"
   },
   {
    "duration": 1004,
    "start_time": "2022-03-14T11:20:47.160Z"
   },
   {
    "duration": 91,
    "start_time": "2022-03-14T11:21:23.527Z"
   },
   {
    "duration": 1076,
    "start_time": "2022-03-14T11:21:32.825Z"
   },
   {
    "duration": 100,
    "start_time": "2022-03-14T11:23:56.776Z"
   },
   {
    "duration": 1040,
    "start_time": "2022-03-14T11:24:02.130Z"
   },
   {
    "duration": 1015,
    "start_time": "2022-03-14T11:24:38.104Z"
   },
   {
    "duration": 1287,
    "start_time": "2022-03-14T11:25:03.655Z"
   },
   {
    "duration": 1045,
    "start_time": "2022-03-14T11:25:18.506Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-14T11:29:13.655Z"
   },
   {
    "duration": 969,
    "start_time": "2022-03-14T11:29:15.611Z"
   },
   {
    "duration": 1404,
    "start_time": "2022-03-14T11:31:01.367Z"
   },
   {
    "duration": 1001,
    "start_time": "2022-03-14T11:32:42.055Z"
   },
   {
    "duration": 4118,
    "start_time": "2022-03-14T11:33:15.689Z"
   },
   {
    "duration": 3115,
    "start_time": "2022-03-14T11:33:29.046Z"
   },
   {
    "duration": 1016,
    "start_time": "2022-03-14T11:37:38.134Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-14T11:39:37.654Z"
   },
   {
    "duration": 3209,
    "start_time": "2022-03-14T11:39:39.092Z"
   },
   {
    "duration": 89,
    "start_time": "2022-03-14T11:48:23.525Z"
   },
   {
    "duration": 1053,
    "start_time": "2022-03-14T11:48:31.570Z"
   },
   {
    "duration": 1385,
    "start_time": "2022-03-14T11:48:56.466Z"
   },
   {
    "duration": 9,
    "start_time": "2022-03-14T11:51:08.179Z"
   },
   {
    "duration": 1619,
    "start_time": "2022-03-14T11:51:10.805Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-14T11:51:44.306Z"
   },
   {
    "duration": 3164,
    "start_time": "2022-03-14T11:51:47.444Z"
   },
   {
    "duration": 95,
    "start_time": "2022-03-14T11:52:40.180Z"
   },
   {
    "duration": 3091,
    "start_time": "2022-03-14T11:52:53.236Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-14T11:53:50.882Z"
   },
   {
    "duration": 3113,
    "start_time": "2022-03-14T11:53:52.066Z"
   },
   {
    "duration": 1351,
    "start_time": "2022-03-14T12:08:34.539Z"
   },
   {
    "duration": 495,
    "start_time": "2022-03-14T12:08:35.893Z"
   },
   {
    "duration": 40,
    "start_time": "2022-03-14T12:08:36.390Z"
   },
   {
    "duration": 187,
    "start_time": "2022-03-14T12:08:36.432Z"
   },
   {
    "duration": 166,
    "start_time": "2022-03-14T12:08:36.622Z"
   },
   {
    "duration": 1711,
    "start_time": "2022-03-14T12:08:36.790Z"
   },
   {
    "duration": 7459,
    "start_time": "2022-03-14T12:08:38.505Z"
   },
   {
    "duration": 2615,
    "start_time": "2022-03-14T12:08:45.967Z"
   },
   {
    "duration": 2583,
    "start_time": "2022-03-14T12:08:48.584Z"
   },
   {
    "duration": 2547,
    "start_time": "2022-03-14T12:08:51.169Z"
   },
   {
    "duration": 82,
    "start_time": "2022-03-14T12:08:53.719Z"
   },
   {
    "duration": 115,
    "start_time": "2022-03-14T12:08:53.804Z"
   },
   {
    "duration": 228,
    "start_time": "2022-03-14T12:08:53.921Z"
   },
   {
    "duration": 72,
    "start_time": "2022-03-14T12:08:54.152Z"
   },
   {
    "duration": 114,
    "start_time": "2022-03-14T12:08:54.226Z"
   },
   {
    "duration": 159,
    "start_time": "2022-03-14T12:08:54.342Z"
   },
   {
    "duration": 738,
    "start_time": "2022-03-14T12:08:54.503Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-14T12:08:55.244Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-14T12:08:55.266Z"
   },
   {
    "duration": 44,
    "start_time": "2022-03-14T12:08:55.302Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-14T12:08:55.349Z"
   },
   {
    "duration": 3314,
    "start_time": "2022-03-14T12:08:55.359Z"
   },
   {
    "duration": 697,
    "start_time": "2022-03-14T12:11:27.159Z"
   },
   {
    "duration": 698,
    "start_time": "2022-03-14T12:11:35.479Z"
   },
   {
    "duration": 674,
    "start_time": "2022-03-14T12:12:07.319Z"
   },
   {
    "duration": 1282,
    "start_time": "2022-03-14T12:12:23.244Z"
   },
   {
    "duration": 435,
    "start_time": "2022-03-14T12:12:24.528Z"
   },
   {
    "duration": 48,
    "start_time": "2022-03-14T12:12:24.965Z"
   },
   {
    "duration": 143,
    "start_time": "2022-03-14T12:12:25.016Z"
   },
   {
    "duration": 194,
    "start_time": "2022-03-14T12:12:25.162Z"
   },
   {
    "duration": 2315,
    "start_time": "2022-03-14T12:12:25.358Z"
   },
   {
    "duration": 8078,
    "start_time": "2022-03-14T12:12:27.676Z"
   },
   {
    "duration": 2525,
    "start_time": "2022-03-14T12:12:35.758Z"
   },
   {
    "duration": 2744,
    "start_time": "2022-03-14T12:12:38.286Z"
   },
   {
    "duration": 2750,
    "start_time": "2022-03-14T12:12:41.033Z"
   },
   {
    "duration": 52,
    "start_time": "2022-03-14T12:12:43.785Z"
   },
   {
    "duration": 127,
    "start_time": "2022-03-14T12:12:43.902Z"
   },
   {
    "duration": 191,
    "start_time": "2022-03-14T12:12:44.032Z"
   },
   {
    "duration": 197,
    "start_time": "2022-03-14T12:12:44.225Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-14T12:12:44.424Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-14T12:12:44.434Z"
   },
   {
    "duration": 738,
    "start_time": "2022-03-14T12:12:44.621Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-14T12:12:45.362Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-14T12:12:45.378Z"
   },
   {
    "duration": 43,
    "start_time": "2022-03-14T12:12:45.383Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-14T12:12:45.429Z"
   },
   {
    "duration": 3142,
    "start_time": "2022-03-14T12:12:45.437Z"
   },
   {
    "duration": 12839,
    "start_time": "2022-03-15T05:21:52.385Z"
   },
   {
    "duration": 2051,
    "start_time": "2022-03-15T05:22:24.786Z"
   },
   {
    "duration": 409,
    "start_time": "2022-03-15T05:22:26.839Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-15T05:22:27.250Z"
   },
   {
    "duration": 129,
    "start_time": "2022-03-15T05:22:27.301Z"
   },
   {
    "duration": 153,
    "start_time": "2022-03-15T05:22:27.432Z"
   },
   {
    "duration": 1506,
    "start_time": "2022-03-15T05:22:27.587Z"
   },
   {
    "duration": 6160,
    "start_time": "2022-03-15T05:22:29.095Z"
   },
   {
    "duration": 2070,
    "start_time": "2022-03-15T05:22:35.258Z"
   },
   {
    "duration": 1982,
    "start_time": "2022-03-15T05:22:37.330Z"
   },
   {
    "duration": 2139,
    "start_time": "2022-03-15T05:22:39.314Z"
   },
   {
    "duration": 759,
    "start_time": "2022-03-15T05:25:05.359Z"
   },
   {
    "duration": 6836,
    "start_time": "2022-03-15T05:25:22.671Z"
   },
   {
    "duration": 7183,
    "start_time": "2022-03-15T05:26:09.104Z"
   },
   {
    "duration": 79,
    "start_time": "2022-03-15T05:28:40.927Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-15T05:36:16.697Z"
   },
   {
    "duration": 432,
    "start_time": "2022-03-15T05:36:16.703Z"
   },
   {
    "duration": 29,
    "start_time": "2022-03-15T05:36:17.138Z"
   },
   {
    "duration": 147,
    "start_time": "2022-03-15T05:36:17.169Z"
   },
   {
    "duration": 159,
    "start_time": "2022-03-15T05:36:17.318Z"
   },
   {
    "duration": 1825,
    "start_time": "2022-03-15T05:36:17.479Z"
   },
   {
    "duration": 6287,
    "start_time": "2022-03-15T05:36:19.306Z"
   },
   {
    "duration": 2081,
    "start_time": "2022-03-15T05:36:25.597Z"
   },
   {
    "duration": 2182,
    "start_time": "2022-03-15T05:36:27.681Z"
   },
   {
    "duration": 2193,
    "start_time": "2022-03-15T05:36:29.866Z"
   },
   {
    "duration": 6394,
    "start_time": "2022-03-15T05:36:32.061Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-15T05:36:38.457Z"
   },
   {
    "duration": 201,
    "start_time": "2022-03-15T05:36:38.502Z"
   },
   {
    "duration": 117,
    "start_time": "2022-03-15T05:36:38.706Z"
   },
   {
    "duration": 103,
    "start_time": "2022-03-15T05:36:38.901Z"
   },
   {
    "duration": 11,
    "start_time": "2022-03-15T05:36:39.007Z"
   },
   {
    "duration": 126,
    "start_time": "2022-03-15T05:36:39.020Z"
   },
   {
    "duration": 629,
    "start_time": "2022-03-15T05:36:39.148Z"
   },
   {
    "duration": 24,
    "start_time": "2022-03-15T05:36:39.779Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T05:36:39.805Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-15T05:37:24.877Z"
   },
   {
    "duration": 83,
    "start_time": "2022-03-15T05:38:24.286Z"
   },
   {
    "duration": 86,
    "start_time": "2022-03-15T05:39:07.199Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T05:39:17.677Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T05:40:17.714Z"
   },
   {
    "duration": 1744,
    "start_time": "2022-03-15T05:40:24.607Z"
   },
   {
    "duration": 1759,
    "start_time": "2022-03-15T05:43:34.493Z"
   },
   {
    "duration": 1734,
    "start_time": "2022-03-15T05:46:48.333Z"
   },
   {
    "duration": 1742,
    "start_time": "2022-03-15T05:47:39.261Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T05:48:27.133Z"
   },
   {
    "duration": 1570,
    "start_time": "2022-03-15T05:48:30.253Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-15T05:50:19.212Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-15T05:50:37.053Z"
   },
   {
    "duration": 1559,
    "start_time": "2022-03-15T06:43:55.446Z"
   },
   {
    "duration": 1386,
    "start_time": "2022-03-15T06:44:30.822Z"
   },
   {
    "duration": 6133,
    "start_time": "2022-03-15T06:48:40.614Z"
   },
   {
    "duration": 99,
    "start_time": "2022-03-15T06:56:16.981Z"
   },
   {
    "duration": 244,
    "start_time": "2022-03-15T06:56:46.839Z"
   },
   {
    "duration": 2601,
    "start_time": "2022-03-15T06:58:05.109Z"
   },
   {
    "duration": 1734,
    "start_time": "2022-03-15T06:58:44.933Z"
   },
   {
    "duration": 809,
    "start_time": "2022-03-15T06:59:24.820Z"
   },
   {
    "duration": 762,
    "start_time": "2022-03-15T07:01:12.181Z"
   },
   {
    "duration": 1822,
    "start_time": "2022-03-15T07:02:06.868Z"
   },
   {
    "duration": 1743,
    "start_time": "2022-03-15T07:02:48.053Z"
   },
   {
    "duration": 1578,
    "start_time": "2022-03-15T07:03:38.869Z"
   },
   {
    "duration": 1772,
    "start_time": "2022-03-15T07:04:29.589Z"
   },
   {
    "duration": 1519,
    "start_time": "2022-03-15T07:08:15.462Z"
   },
   {
    "duration": 1592,
    "start_time": "2022-03-15T07:08:32.181Z"
   },
   {
    "duration": 1503,
    "start_time": "2022-03-15T07:09:27.637Z"
   },
   {
    "duration": 1322,
    "start_time": "2022-03-15T07:10:17.556Z"
   },
   {
    "duration": 1572,
    "start_time": "2022-03-15T07:10:39.717Z"
   },
   {
    "duration": 1319,
    "start_time": "2022-03-15T07:11:08.589Z"
   },
   {
    "duration": 78,
    "start_time": "2022-03-15T07:14:06.228Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-15T07:14:34.276Z"
   },
   {
    "duration": 1399,
    "start_time": "2022-03-15T07:14:59.987Z"
   },
   {
    "duration": 2857,
    "start_time": "2022-03-15T07:15:19.027Z"
   },
   {
    "duration": 2934,
    "start_time": "2022-03-15T07:15:55.044Z"
   },
   {
    "duration": 88,
    "start_time": "2022-03-15T07:25:24.228Z"
   },
   {
    "duration": 253,
    "start_time": "2022-03-15T07:25:39.794Z"
   },
   {
    "duration": 3160,
    "start_time": "2022-03-15T07:26:02.818Z"
   },
   {
    "duration": 114,
    "start_time": "2022-03-15T07:26:34.707Z"
   },
   {
    "duration": 2891,
    "start_time": "2022-03-15T07:26:54.564Z"
   },
   {
    "duration": 2897,
    "start_time": "2022-03-15T07:27:04.659Z"
   },
   {
    "duration": 2985,
    "start_time": "2022-03-15T07:27:27.283Z"
   },
   {
    "duration": 1941,
    "start_time": "2022-03-15T07:28:15.555Z"
   },
   {
    "duration": 2697,
    "start_time": "2022-03-15T07:28:27.749Z"
   },
   {
    "duration": 1795,
    "start_time": "2022-03-15T07:28:57.107Z"
   },
   {
    "duration": 2998,
    "start_time": "2022-03-15T07:29:05.139Z"
   },
   {
    "duration": 76,
    "start_time": "2022-03-15T07:30:36.563Z"
   },
   {
    "duration": 74,
    "start_time": "2022-03-15T07:30:52.754Z"
   },
   {
    "duration": 2933,
    "start_time": "2022-03-15T07:31:09.698Z"
   },
   {
    "duration": 2898,
    "start_time": "2022-03-15T07:31:48.466Z"
   },
   {
    "duration": 2983,
    "start_time": "2022-03-15T07:32:15.394Z"
   },
   {
    "duration": 80,
    "start_time": "2022-03-15T07:32:48.787Z"
   },
   {
    "duration": 2853,
    "start_time": "2022-03-15T07:32:56.051Z"
   },
   {
    "duration": 2930,
    "start_time": "2022-03-15T07:33:19.218Z"
   },
   {
    "duration": 2989,
    "start_time": "2022-03-15T07:34:05.922Z"
   },
   {
    "duration": 2891,
    "start_time": "2022-03-15T07:34:33.522Z"
   },
   {
    "duration": 2885,
    "start_time": "2022-03-15T07:35:57.064Z"
   },
   {
    "duration": 1882,
    "start_time": "2022-03-15T07:36:42.946Z"
   },
   {
    "duration": 2894,
    "start_time": "2022-03-15T07:37:32.835Z"
   },
   {
    "duration": 79,
    "start_time": "2022-03-15T07:39:19.185Z"
   },
   {
    "duration": 3057,
    "start_time": "2022-03-15T07:39:32.433Z"
   },
   {
    "duration": 2858,
    "start_time": "2022-03-15T07:39:57.011Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-15T11:51:50.934Z"
   },
   {
    "duration": 423,
    "start_time": "2022-03-15T11:51:50.942Z"
   },
   {
    "duration": 34,
    "start_time": "2022-03-15T11:51:51.367Z"
   },
   {
    "duration": 127,
    "start_time": "2022-03-15T11:51:51.403Z"
   },
   {
    "duration": 170,
    "start_time": "2022-03-15T11:51:51.533Z"
   },
   {
    "duration": 1455,
    "start_time": "2022-03-15T11:51:51.705Z"
   },
   {
    "duration": 8019,
    "start_time": "2022-03-15T11:51:53.162Z"
   },
   {
    "duration": 2597,
    "start_time": "2022-03-15T11:52:01.184Z"
   },
   {
    "duration": 2430,
    "start_time": "2022-03-15T11:52:03.783Z"
   },
   {
    "duration": 2369,
    "start_time": "2022-03-15T11:52:06.216Z"
   },
   {
    "duration": 6174,
    "start_time": "2022-03-15T11:52:08.588Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-15T11:52:14.765Z"
   },
   {
    "duration": 206,
    "start_time": "2022-03-15T11:52:14.805Z"
   },
   {
    "duration": 195,
    "start_time": "2022-03-15T11:52:15.015Z"
   },
   {
    "duration": 191,
    "start_time": "2022-03-15T11:52:15.213Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-15T11:52:15.407Z"
   },
   {
    "duration": 139,
    "start_time": "2022-03-15T11:52:15.421Z"
   },
   {
    "duration": 618,
    "start_time": "2022-03-15T11:52:15.563Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-15T11:52:16.183Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-15T11:52:21.220Z"
   },
   {
    "duration": 538,
    "start_time": "2022-03-15T11:52:48.451Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-15T11:53:35.412Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-15T11:54:06.548Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-15T11:55:02.996Z"
   },
   {
    "duration": 676,
    "start_time": "2022-03-15T11:55:09.493Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-15T11:56:05.687Z"
   },
   {
    "duration": 3738,
    "start_time": "2022-03-15T11:56:18.356Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-15T11:56:37.299Z"
   },
   {
    "duration": 470,
    "start_time": "2022-03-15T11:56:40.238Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-15T11:59:53.911Z"
   },
   {
    "duration": 329,
    "start_time": "2022-03-15T11:59:55.557Z"
   },
   {
    "duration": 1350,
    "start_time": "2022-03-15T12:00:08.068Z"
   },
   {
    "duration": 800,
    "start_time": "2022-03-15T12:00:51.795Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-15T12:02:36.421Z"
   },
   {
    "duration": 734,
    "start_time": "2022-03-15T12:02:37.059Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-15T12:04:19.620Z"
   },
   {
    "duration": 749,
    "start_time": "2022-03-15T12:04:20.374Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-15T12:08:03.332Z"
   },
   {
    "duration": 520,
    "start_time": "2022-03-15T12:08:06.771Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-15T12:08:59.538Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-15T12:09:02.468Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-15T12:09:36.755Z"
   },
   {
    "duration": 3526,
    "start_time": "2022-03-15T12:09:45.219Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-15T12:12:25.123Z"
   },
   {
    "duration": 3433,
    "start_time": "2022-03-15T12:12:31.763Z"
   },
   {
    "duration": 1782,
    "start_time": "2022-03-15T12:20:26.325Z"
   },
   {
    "duration": 435,
    "start_time": "2022-03-15T12:20:28.110Z"
   },
   {
    "duration": 29,
    "start_time": "2022-03-15T12:20:28.548Z"
   },
   {
    "duration": 137,
    "start_time": "2022-03-15T12:20:28.601Z"
   },
   {
    "duration": 192,
    "start_time": "2022-03-15T12:20:28.740Z"
   },
   {
    "duration": 1601,
    "start_time": "2022-03-15T12:20:28.934Z"
   },
   {
    "duration": 6916,
    "start_time": "2022-03-15T12:20:30.537Z"
   },
   {
    "duration": 2309,
    "start_time": "2022-03-15T12:20:37.457Z"
   },
   {
    "duration": 2272,
    "start_time": "2022-03-15T12:20:39.770Z"
   },
   {
    "duration": 2137,
    "start_time": "2022-03-15T12:20:42.044Z"
   },
   {
    "duration": 7309,
    "start_time": "2022-03-15T12:20:44.183Z"
   },
   {
    "duration": 108,
    "start_time": "2022-03-15T12:20:51.494Z"
   },
   {
    "duration": 123,
    "start_time": "2022-03-15T12:20:51.610Z"
   },
   {
    "duration": 177,
    "start_time": "2022-03-15T12:20:51.736Z"
   },
   {
    "duration": 218,
    "start_time": "2022-03-15T12:20:51.917Z"
   },
   {
    "duration": 32,
    "start_time": "2022-03-15T12:20:52.137Z"
   },
   {
    "duration": 147,
    "start_time": "2022-03-15T12:20:52.171Z"
   },
   {
    "duration": 656,
    "start_time": "2022-03-15T12:20:52.321Z"
   },
   {
    "duration": 28,
    "start_time": "2022-03-15T12:20:52.979Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-15T12:20:53.010Z"
   },
   {
    "duration": 46,
    "start_time": "2022-03-15T12:20:53.019Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T12:20:53.067Z"
   },
   {
    "duration": 314,
    "start_time": "2022-03-15T12:20:53.076Z"
   },
   {
    "duration": -89,
    "start_time": "2022-03-15T12:20:53.481Z"
   },
   {
    "duration": -90,
    "start_time": "2022-03-15T12:20:53.483Z"
   },
   {
    "duration": 3261,
    "start_time": "2022-03-15T12:23:15.523Z"
   },
   {
    "duration": 13,
    "start_time": "2022-03-15T12:23:29.107Z"
   },
   {
    "duration": 4021,
    "start_time": "2022-03-15T12:23:30.085Z"
   },
   {
    "duration": 1782,
    "start_time": "2022-03-15T12:23:58.820Z"
   },
   {
    "duration": 454,
    "start_time": "2022-03-15T12:24:00.604Z"
   },
   {
    "duration": 51,
    "start_time": "2022-03-15T12:24:01.061Z"
   },
   {
    "duration": 142,
    "start_time": "2022-03-15T12:24:01.115Z"
   },
   {
    "duration": 186,
    "start_time": "2022-03-15T12:24:01.258Z"
   },
   {
    "duration": 1613,
    "start_time": "2022-03-15T12:24:01.446Z"
   },
   {
    "duration": 7334,
    "start_time": "2022-03-15T12:24:03.061Z"
   },
   {
    "duration": 2369,
    "start_time": "2022-03-15T12:24:10.398Z"
   },
   {
    "duration": 2343,
    "start_time": "2022-03-15T12:24:12.771Z"
   },
   {
    "duration": 2314,
    "start_time": "2022-03-15T12:24:15.117Z"
   },
   {
    "duration": 7206,
    "start_time": "2022-03-15T12:24:17.433Z"
   },
   {
    "duration": 67,
    "start_time": "2022-03-15T12:24:24.642Z"
   },
   {
    "duration": 191,
    "start_time": "2022-03-15T12:24:24.712Z"
   },
   {
    "duration": 115,
    "start_time": "2022-03-15T12:24:24.912Z"
   },
   {
    "duration": 172,
    "start_time": "2022-03-15T12:24:25.030Z"
   },
   {
    "duration": 25,
    "start_time": "2022-03-15T12:24:25.204Z"
   },
   {
    "duration": 126,
    "start_time": "2022-03-15T12:24:25.231Z"
   },
   {
    "duration": 643,
    "start_time": "2022-03-15T12:24:25.359Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-15T12:24:26.005Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T12:24:26.026Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-15T12:24:26.033Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-15T12:24:26.057Z"
   },
   {
    "duration": 3113,
    "start_time": "2022-03-15T12:24:26.065Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-15T12:24:29.179Z"
   },
   {
    "duration": 3173,
    "start_time": "2022-03-15T12:24:29.188Z"
   },
   {
    "duration": 1122,
    "start_time": "2022-03-16T04:38:20.209Z"
   },
   {
    "duration": 369,
    "start_time": "2022-03-16T04:38:21.333Z"
   },
   {
    "duration": 24,
    "start_time": "2022-03-16T04:38:21.704Z"
   },
   {
    "duration": 109,
    "start_time": "2022-03-16T04:38:21.729Z"
   },
   {
    "duration": 135,
    "start_time": "2022-03-16T04:38:21.840Z"
   },
   {
    "duration": 1358,
    "start_time": "2022-03-16T04:38:21.977Z"
   },
   {
    "duration": 5578,
    "start_time": "2022-03-16T04:38:23.336Z"
   },
   {
    "duration": 1883,
    "start_time": "2022-03-16T04:38:28.916Z"
   },
   {
    "duration": 1903,
    "start_time": "2022-03-16T04:38:30.802Z"
   },
   {
    "duration": 1930,
    "start_time": "2022-03-16T04:38:32.707Z"
   },
   {
    "duration": 207,
    "start_time": "2022-03-16T04:38:34.639Z"
   },
   {
    "duration": -47,
    "start_time": "2022-03-16T04:38:34.894Z"
   },
   {
    "duration": -48,
    "start_time": "2022-03-16T04:38:34.896Z"
   },
   {
    "duration": -49,
    "start_time": "2022-03-16T04:38:34.898Z"
   },
   {
    "duration": -81,
    "start_time": "2022-03-16T04:38:34.931Z"
   },
   {
    "duration": -81,
    "start_time": "2022-03-16T04:38:34.932Z"
   },
   {
    "duration": -82,
    "start_time": "2022-03-16T04:38:34.934Z"
   },
   {
    "duration": -84,
    "start_time": "2022-03-16T04:38:34.936Z"
   },
   {
    "duration": -84,
    "start_time": "2022-03-16T04:38:34.937Z"
   },
   {
    "duration": -85,
    "start_time": "2022-03-16T04:38:34.939Z"
   },
   {
    "duration": -86,
    "start_time": "2022-03-16T04:38:34.941Z"
   },
   {
    "duration": -86,
    "start_time": "2022-03-16T04:38:34.942Z"
   },
   {
    "duration": -88,
    "start_time": "2022-03-16T04:38:34.945Z"
   },
   {
    "duration": -88,
    "start_time": "2022-03-16T04:38:34.946Z"
   },
   {
    "duration": -89,
    "start_time": "2022-03-16T04:38:34.948Z"
   },
   {
    "duration": 244,
    "start_time": "2022-03-16T04:41:37.004Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-16T04:41:46.423Z"
   },
   {
    "duration": 392,
    "start_time": "2022-03-16T04:41:46.431Z"
   },
   {
    "duration": 40,
    "start_time": "2022-03-16T04:41:46.825Z"
   },
   {
    "duration": 127,
    "start_time": "2022-03-16T04:41:46.867Z"
   },
   {
    "duration": 134,
    "start_time": "2022-03-16T04:41:46.997Z"
   },
   {
    "duration": 1315,
    "start_time": "2022-03-16T04:41:47.133Z"
   },
   {
    "duration": 5391,
    "start_time": "2022-03-16T04:41:48.451Z"
   },
   {
    "duration": 1805,
    "start_time": "2022-03-16T04:41:53.844Z"
   },
   {
    "duration": 1935,
    "start_time": "2022-03-16T04:41:55.652Z"
   },
   {
    "duration": 1842,
    "start_time": "2022-03-16T04:41:57.589Z"
   },
   {
    "duration": 206,
    "start_time": "2022-03-16T04:41:59.433Z"
   },
   {
    "duration": -45,
    "start_time": "2022-03-16T04:41:59.686Z"
   },
   {
    "duration": -45,
    "start_time": "2022-03-16T04:41:59.687Z"
   },
   {
    "duration": -49,
    "start_time": "2022-03-16T04:41:59.692Z"
   },
   {
    "duration": -77,
    "start_time": "2022-03-16T04:41:59.721Z"
   },
   {
    "duration": -82,
    "start_time": "2022-03-16T04:41:59.727Z"
   },
   {
    "duration": -84,
    "start_time": "2022-03-16T04:41:59.730Z"
   },
   {
    "duration": -85,
    "start_time": "2022-03-16T04:41:59.732Z"
   },
   {
    "duration": -87,
    "start_time": "2022-03-16T04:41:59.735Z"
   },
   {
    "duration": -88,
    "start_time": "2022-03-16T04:41:59.737Z"
   },
   {
    "duration": -89,
    "start_time": "2022-03-16T04:41:59.739Z"
   },
   {
    "duration": -89,
    "start_time": "2022-03-16T04:41:59.740Z"
   },
   {
    "duration": -92,
    "start_time": "2022-03-16T04:41:59.744Z"
   },
   {
    "duration": -93,
    "start_time": "2022-03-16T04:41:59.746Z"
   },
   {
    "duration": -94,
    "start_time": "2022-03-16T04:41:59.748Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-16T04:43:26.505Z"
   },
   {
    "duration": 391,
    "start_time": "2022-03-16T04:43:26.511Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-16T04:43:26.903Z"
   },
   {
    "duration": 121,
    "start_time": "2022-03-16T04:43:26.925Z"
   },
   {
    "duration": 109,
    "start_time": "2022-03-16T04:43:27.064Z"
   },
   {
    "duration": 1413,
    "start_time": "2022-03-16T04:43:27.174Z"
   },
   {
    "duration": 5560,
    "start_time": "2022-03-16T04:43:28.589Z"
   },
   {
    "duration": 1907,
    "start_time": "2022-03-16T04:43:34.151Z"
   },
   {
    "duration": 1891,
    "start_time": "2022-03-16T04:43:36.061Z"
   },
   {
    "duration": 1789,
    "start_time": "2022-03-16T04:43:37.954Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-16T04:43:39.745Z"
   },
   {
    "duration": 204,
    "start_time": "2022-03-16T04:43:39.770Z"
   },
   {
    "duration": 195,
    "start_time": "2022-03-16T04:43:39.976Z"
   },
   {
    "duration": 191,
    "start_time": "2022-03-16T04:43:40.174Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-16T04:43:40.367Z"
   },
   {
    "duration": 125,
    "start_time": "2022-03-16T04:43:40.373Z"
   },
   {
    "duration": 553,
    "start_time": "2022-03-16T04:43:40.500Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-16T04:43:41.055Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-16T04:43:41.075Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-16T04:43:41.080Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-16T04:43:41.104Z"
   },
   {
    "duration": 4628,
    "start_time": "2022-03-16T04:43:41.110Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-16T04:43:45.740Z"
   },
   {
    "duration": 5400,
    "start_time": "2022-03-16T04:43:45.748Z"
   },
   {
    "duration": 5040,
    "start_time": "2022-03-16T04:44:22.491Z"
   },
   {
    "duration": 1103,
    "start_time": "2022-03-16T04:44:47.319Z"
   },
   {
    "duration": 371,
    "start_time": "2022-03-16T04:44:48.424Z"
   },
   {
    "duration": 25,
    "start_time": "2022-03-16T04:44:48.797Z"
   },
   {
    "duration": 122,
    "start_time": "2022-03-16T04:44:48.824Z"
   },
   {
    "duration": 133,
    "start_time": "2022-03-16T04:44:48.947Z"
   },
   {
    "duration": 1384,
    "start_time": "2022-03-16T04:44:49.081Z"
   },
   {
    "duration": 5605,
    "start_time": "2022-03-16T04:44:50.466Z"
   },
   {
    "duration": 1761,
    "start_time": "2022-03-16T04:44:56.074Z"
   },
   {
    "duration": 1755,
    "start_time": "2022-03-16T04:44:57.837Z"
   },
   {
    "duration": 1904,
    "start_time": "2022-03-16T04:44:59.594Z"
   },
   {
    "duration": 74,
    "start_time": "2022-03-16T04:45:01.499Z"
   },
   {
    "duration": 26,
    "start_time": "2022-03-16T04:45:01.664Z"
   },
   {
    "duration": 188,
    "start_time": "2022-03-16T04:45:01.693Z"
   },
   {
    "duration": 187,
    "start_time": "2022-03-16T04:45:01.884Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-16T04:45:02.073Z"
   },
   {
    "duration": 137,
    "start_time": "2022-03-16T04:45:02.080Z"
   },
   {
    "duration": 573,
    "start_time": "2022-03-16T04:45:02.219Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-16T04:45:02.795Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-16T04:45:02.811Z"
   },
   {
    "duration": 49,
    "start_time": "2022-03-16T04:45:02.817Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-16T04:45:02.868Z"
   },
   {
    "duration": 4788,
    "start_time": "2022-03-16T04:45:02.875Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-16T04:45:07.667Z"
   },
   {
    "duration": 5458,
    "start_time": "2022-03-16T04:45:07.675Z"
   },
   {
    "duration": 4936,
    "start_time": "2022-03-16T04:46:01.435Z"
   },
   {
    "duration": 206,
    "start_time": "2022-03-16T04:49:26.927Z"
   },
   {
    "duration": 4717,
    "start_time": "2022-03-16T04:49:51.482Z"
   },
   {
    "duration": 4592,
    "start_time": "2022-03-16T04:50:22.042Z"
   },
   {
    "duration": 4768,
    "start_time": "2022-03-16T04:50:36.164Z"
   },
   {
    "duration": 4709,
    "start_time": "2022-03-16T04:52:09.962Z"
   },
   {
    "duration": 4860,
    "start_time": "2022-03-16T04:53:26.314Z"
   },
   {
    "duration": 9277,
    "start_time": "2022-03-16T05:08:17.736Z"
   },
   {
    "duration": 4716,
    "start_time": "2022-03-16T05:09:51.817Z"
   },
   {
    "duration": 4626,
    "start_time": "2022-03-16T05:10:03.769Z"
   },
   {
    "duration": 4734,
    "start_time": "2022-03-16T05:12:15.290Z"
   },
   {
    "duration": 4596,
    "start_time": "2022-03-16T05:12:31.545Z"
   },
   {
    "duration": 4729,
    "start_time": "2022-03-16T05:13:51.753Z"
   },
   {
    "duration": 4776,
    "start_time": "2022-03-16T05:14:10.792Z"
   },
   {
    "duration": 4892,
    "start_time": "2022-03-16T05:14:27.336Z"
   },
   {
    "duration": 70,
    "start_time": "2022-03-16T05:16:30.776Z"
   },
   {
    "duration": 4777,
    "start_time": "2022-03-16T05:16:43.449Z"
   },
   {
    "duration": 4748,
    "start_time": "2022-03-16T05:17:35.160Z"
   },
   {
    "duration": 4911,
    "start_time": "2022-03-16T05:21:15.512Z"
   },
   {
    "duration": 4540,
    "start_time": "2022-03-16T05:22:55.048Z"
   },
   {
    "duration": 207,
    "start_time": "2022-03-16T05:23:55.161Z"
   },
   {
    "duration": 4755,
    "start_time": "2022-03-16T05:24:11.049Z"
   },
   {
    "duration": 4697,
    "start_time": "2022-03-16T05:25:21.370Z"
   },
   {
    "duration": 4841,
    "start_time": "2022-03-16T05:25:43.879Z"
   },
   {
    "duration": 4986,
    "start_time": "2022-03-16T05:26:43.207Z"
   },
   {
    "duration": 4710,
    "start_time": "2022-03-16T05:27:04.520Z"
   },
   {
    "duration": 4896,
    "start_time": "2022-03-16T05:27:29.463Z"
   },
   {
    "duration": 5206,
    "start_time": "2022-03-16T05:29:54.839Z"
   },
   {
    "duration": 5370,
    "start_time": "2022-03-16T05:30:12.871Z"
   },
   {
    "duration": 6984,
    "start_time": "2022-03-16T05:32:34.696Z"
   },
   {
    "duration": 6944,
    "start_time": "2022-03-16T05:33:08.760Z"
   },
   {
    "duration": 73,
    "start_time": "2022-03-16T05:34:36.999Z"
   },
   {
    "duration": 4732,
    "start_time": "2022-03-16T05:35:48.470Z"
   },
   {
    "duration": 1227,
    "start_time": "2022-03-16T05:36:31.318Z"
   },
   {
    "duration": 391,
    "start_time": "2022-03-16T05:36:32.547Z"
   },
   {
    "duration": 41,
    "start_time": "2022-03-16T05:36:32.940Z"
   },
   {
    "duration": 138,
    "start_time": "2022-03-16T05:36:32.983Z"
   },
   {
    "duration": 131,
    "start_time": "2022-03-16T05:36:33.123Z"
   },
   {
    "duration": 1472,
    "start_time": "2022-03-16T05:36:33.262Z"
   },
   {
    "duration": 5620,
    "start_time": "2022-03-16T05:36:34.736Z"
   },
   {
    "duration": 1900,
    "start_time": "2022-03-16T05:36:40.360Z"
   },
   {
    "duration": 2085,
    "start_time": "2022-03-16T05:36:42.263Z"
   },
   {
    "duration": 1910,
    "start_time": "2022-03-16T05:36:44.350Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-16T05:36:46.261Z"
   },
   {
    "duration": 116,
    "start_time": "2022-03-16T05:36:46.365Z"
   },
   {
    "duration": 192,
    "start_time": "2022-03-16T05:36:46.483Z"
   },
   {
    "duration": 97,
    "start_time": "2022-03-16T05:36:46.677Z"
   },
   {
    "duration": 31,
    "start_time": "2022-03-16T05:36:46.862Z"
   },
   {
    "duration": 115,
    "start_time": "2022-03-16T05:36:46.894Z"
   },
   {
    "duration": 593,
    "start_time": "2022-03-16T05:36:47.011Z"
   },
   {
    "duration": 15,
    "start_time": "2022-03-16T05:36:47.606Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-16T05:36:47.623Z"
   },
   {
    "duration": 43,
    "start_time": "2022-03-16T05:36:47.629Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-16T05:36:47.674Z"
   },
   {
    "duration": 5488,
    "start_time": "2022-03-16T05:36:47.682Z"
   },
   {
    "duration": 8,
    "start_time": "2022-03-16T05:36:53.173Z"
   },
   {
    "duration": 7395,
    "start_time": "2022-03-16T05:36:53.183Z"
   },
   {
    "duration": 53,
    "start_time": "2022-03-18T05:08:14.997Z"
   },
   {
    "duration": 1701,
    "start_time": "2022-03-18T05:08:25.245Z"
   },
   {
    "duration": 379,
    "start_time": "2022-03-18T05:08:26.949Z"
   },
   {
    "duration": 37,
    "start_time": "2022-03-18T05:08:27.330Z"
   },
   {
    "duration": 112,
    "start_time": "2022-03-18T05:08:27.369Z"
   },
   {
    "duration": 131,
    "start_time": "2022-03-18T05:08:27.483Z"
   },
   {
    "duration": 918,
    "start_time": "2022-03-18T05:08:27.616Z"
   },
   {
    "duration": 441,
    "start_time": "2022-03-18T05:08:28.535Z"
   },
   {
    "duration": 170,
    "start_time": "2022-03-18T05:08:28.977Z"
   },
   {
    "duration": 165,
    "start_time": "2022-03-18T05:08:29.149Z"
   },
   {
    "duration": 175,
    "start_time": "2022-03-18T05:08:29.315Z"
   },
   {
    "duration": 173,
    "start_time": "2022-03-18T05:08:29.492Z"
   },
   {
    "duration": 113,
    "start_time": "2022-03-18T05:08:29.765Z"
   },
   {
    "duration": 204,
    "start_time": "2022-03-18T05:08:29.881Z"
   },
   {
    "duration": 178,
    "start_time": "2022-03-18T05:08:30.090Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-18T05:08:30.269Z"
   },
   {
    "duration": 133,
    "start_time": "2022-03-18T05:08:30.294Z"
   },
   {
    "duration": 436,
    "start_time": "2022-03-18T05:08:30.429Z"
   },
   {
    "duration": 12,
    "start_time": "2022-03-18T05:08:30.867Z"
   },
   {
    "duration": 24,
    "start_time": "2022-03-18T05:08:30.880Z"
   },
   {
    "duration": 43,
    "start_time": "2022-03-18T05:08:30.906Z"
   },
   {
    "duration": 7,
    "start_time": "2022-03-18T05:08:30.951Z"
   },
   {
    "duration": 2566,
    "start_time": "2022-03-18T05:08:30.959Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T05:08:33.527Z"
   },
   {
    "duration": 2522,
    "start_time": "2022-03-18T05:08:33.535Z"
   },
   {
    "duration": 4332,
    "start_time": "2022-03-18T05:13:38.640Z"
   },
   {
    "duration": 1499,
    "start_time": "2022-03-18T05:13:57.311Z"
   },
   {
    "duration": 2330,
    "start_time": "2022-03-18T05:16:47.615Z"
   },
   {
    "duration": 6093,
    "start_time": "2022-03-18T05:19:02.192Z"
   },
   {
    "duration": 130,
    "start_time": "2022-03-18T05:19:36.912Z"
   },
   {
    "duration": 2337,
    "start_time": "2022-03-18T05:22:11.009Z"
   },
   {
    "duration": 1526,
    "start_time": "2022-03-18T05:24:36.325Z"
   },
   {
    "duration": 400,
    "start_time": "2022-03-18T05:24:37.853Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-18T05:24:38.254Z"
   },
   {
    "duration": 130,
    "start_time": "2022-03-18T05:24:38.292Z"
   },
   {
    "duration": 148,
    "start_time": "2022-03-18T05:24:38.424Z"
   },
   {
    "duration": 920,
    "start_time": "2022-03-18T05:24:38.574Z"
   },
   {
    "duration": 461,
    "start_time": "2022-03-18T05:24:39.495Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-18T05:24:39.962Z"
   },
   {
    "duration": 196,
    "start_time": "2022-03-18T05:24:40.147Z"
   },
   {
    "duration": 185,
    "start_time": "2022-03-18T05:24:40.346Z"
   },
   {
    "duration": 37,
    "start_time": "2022-03-18T05:24:40.532Z"
   },
   {
    "duration": 203,
    "start_time": "2022-03-18T05:24:40.571Z"
   },
   {
    "duration": 200,
    "start_time": "2022-03-18T05:24:40.776Z"
   },
   {
    "duration": 186,
    "start_time": "2022-03-18T05:24:40.978Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T05:24:41.166Z"
   },
   {
    "duration": 133,
    "start_time": "2022-03-18T05:24:41.172Z"
   },
   {
    "duration": 421,
    "start_time": "2022-03-18T05:24:41.307Z"
   },
   {
    "duration": 13,
    "start_time": "2022-03-18T05:24:41.730Z"
   },
   {
    "duration": 21,
    "start_time": "2022-03-18T05:24:41.744Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-18T05:24:41.766Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T05:24:41.786Z"
   },
   {
    "duration": 2815,
    "start_time": "2022-03-18T05:24:41.793Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T05:24:44.610Z"
   },
   {
    "duration": 2586,
    "start_time": "2022-03-18T05:24:44.617Z"
   },
   {
    "duration": 1489,
    "start_time": "2022-03-18T05:25:46.361Z"
   },
   {
    "duration": 394,
    "start_time": "2022-03-18T05:25:47.852Z"
   },
   {
    "duration": 32,
    "start_time": "2022-03-18T05:25:48.248Z"
   },
   {
    "duration": 110,
    "start_time": "2022-03-18T05:25:48.282Z"
   },
   {
    "duration": 144,
    "start_time": "2022-03-18T05:25:48.393Z"
   },
   {
    "duration": 898,
    "start_time": "2022-03-18T05:25:48.539Z"
   },
   {
    "duration": 441,
    "start_time": "2022-03-18T05:25:49.439Z"
   },
   {
    "duration": 182,
    "start_time": "2022-03-18T05:25:49.882Z"
   },
   {
    "duration": 174,
    "start_time": "2022-03-18T05:25:50.066Z"
   },
   {
    "duration": 163,
    "start_time": "2022-03-18T05:25:50.243Z"
   },
   {
    "duration": 29,
    "start_time": "2022-03-18T05:25:50.408Z"
   },
   {
    "duration": 200,
    "start_time": "2022-03-18T05:25:50.464Z"
   },
   {
    "duration": 116,
    "start_time": "2022-03-18T05:25:50.666Z"
   },
   {
    "duration": 180,
    "start_time": "2022-03-18T05:25:50.784Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T05:25:50.965Z"
   },
   {
    "duration": 122,
    "start_time": "2022-03-18T05:25:50.971Z"
   },
   {
    "duration": 413,
    "start_time": "2022-03-18T05:25:51.095Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-18T05:25:51.509Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-18T05:25:51.524Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-18T05:25:51.529Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T05:25:51.567Z"
   },
   {
    "duration": 2553,
    "start_time": "2022-03-18T05:25:51.574Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T05:25:54.129Z"
   },
   {
    "duration": 2590,
    "start_time": "2022-03-18T05:25:54.136Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-18T06:10:19.657Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T06:11:31.403Z"
   },
   {
    "duration": 172,
    "start_time": "2022-03-18T06:12:06.377Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T06:13:12.137Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T06:13:56.025Z"
   },
   {
    "duration": 16,
    "start_time": "2022-03-18T06:14:28.249Z"
   },
   {
    "duration": 255,
    "start_time": "2022-03-18T06:15:26.202Z"
   },
   {
    "duration": 247,
    "start_time": "2022-03-18T06:15:38.953Z"
   },
   {
    "duration": 264,
    "start_time": "2022-03-18T06:17:13.272Z"
   },
   {
    "duration": 392,
    "start_time": "2022-03-18T06:18:04.153Z"
   },
   {
    "duration": 325,
    "start_time": "2022-03-18T06:18:23.866Z"
   },
   {
    "duration": 319,
    "start_time": "2022-03-18T06:18:45.191Z"
   },
   {
    "duration": 328,
    "start_time": "2022-03-18T06:19:40.216Z"
   },
   {
    "duration": 304,
    "start_time": "2022-03-18T06:20:06.985Z"
   },
   {
    "duration": 313,
    "start_time": "2022-03-18T06:23:39.369Z"
   },
   {
    "duration": 453,
    "start_time": "2022-03-18T06:26:01.705Z"
   },
   {
    "duration": 329,
    "start_time": "2022-03-18T06:28:04.361Z"
   },
   {
    "duration": 320,
    "start_time": "2022-03-18T06:28:17.320Z"
   },
   {
    "duration": 342,
    "start_time": "2022-03-18T06:28:45.960Z"
   },
   {
    "duration": 321,
    "start_time": "2022-03-18T06:29:30.344Z"
   },
   {
    "duration": 446,
    "start_time": "2022-03-18T06:29:37.016Z"
   },
   {
    "duration": 313,
    "start_time": "2022-03-18T06:30:27.480Z"
   },
   {
    "duration": 344,
    "start_time": "2022-03-18T06:30:38.072Z"
   },
   {
    "duration": 313,
    "start_time": "2022-03-18T06:30:59.288Z"
   },
   {
    "duration": 1689,
    "start_time": "2022-03-18T06:31:31.449Z"
   },
   {
    "duration": 392,
    "start_time": "2022-03-18T06:31:33.140Z"
   },
   {
    "duration": 35,
    "start_time": "2022-03-18T06:31:33.535Z"
   },
   {
    "duration": 121,
    "start_time": "2022-03-18T06:31:33.572Z"
   },
   {
    "duration": 150,
    "start_time": "2022-03-18T06:31:33.696Z"
   },
   {
    "duration": 375,
    "start_time": "2022-03-18T06:31:33.847Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.224Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.225Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.226Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.226Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.227Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.228Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.229Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.230Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.232Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.233Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.234Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.234Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.235Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.236Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.237Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.262Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.263Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.264Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.266Z"
   },
   {
    "duration": 0,
    "start_time": "2022-03-18T06:31:34.267Z"
   },
   {
    "duration": 1681,
    "start_time": "2022-03-18T06:33:15.479Z"
   },
   {
    "duration": 385,
    "start_time": "2022-03-18T06:33:17.162Z"
   },
   {
    "duration": 30,
    "start_time": "2022-03-18T06:33:17.548Z"
   },
   {
    "duration": 113,
    "start_time": "2022-03-18T06:33:17.579Z"
   },
   {
    "duration": 137,
    "start_time": "2022-03-18T06:33:17.694Z"
   },
   {
    "duration": 321,
    "start_time": "2022-03-18T06:33:17.832Z"
   },
   {
    "duration": 311,
    "start_time": "2022-03-18T06:33:18.154Z"
   },
   {
    "duration": 406,
    "start_time": "2022-03-18T06:33:18.466Z"
   },
   {
    "duration": 425,
    "start_time": "2022-03-18T06:33:18.874Z"
   },
   {
    "duration": 169,
    "start_time": "2022-03-18T06:33:19.301Z"
   },
   {
    "duration": 166,
    "start_time": "2022-03-18T06:33:19.472Z"
   },
   {
    "duration": 163,
    "start_time": "2022-03-18T06:33:19.640Z"
   },
   {
    "duration": 59,
    "start_time": "2022-03-18T06:33:19.804Z"
   },
   {
    "duration": 123,
    "start_time": "2022-03-18T06:33:19.869Z"
   },
   {
    "duration": 119,
    "start_time": "2022-03-18T06:33:20.064Z"
   },
   {
    "duration": 179,
    "start_time": "2022-03-18T06:33:20.186Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T06:33:20.367Z"
   },
   {
    "duration": 118,
    "start_time": "2022-03-18T06:33:20.374Z"
   },
   {
    "duration": 445,
    "start_time": "2022-03-18T06:33:20.494Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-18T06:33:20.941Z"
   },
   {
    "duration": 3,
    "start_time": "2022-03-18T06:33:20.970Z"
   },
   {
    "duration": 20,
    "start_time": "2022-03-18T06:33:20.974Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T06:33:20.996Z"
   },
   {
    "duration": 2610,
    "start_time": "2022-03-18T06:33:21.002Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T06:33:23.614Z"
   },
   {
    "duration": 2665,
    "start_time": "2022-03-18T06:33:23.621Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T06:52:30.824Z"
   },
   {
    "duration": 386,
    "start_time": "2022-03-18T07:05:44.225Z"
   },
   {
    "duration": 23,
    "start_time": "2022-03-18T07:06:10.098Z"
   },
   {
    "duration": 90,
    "start_time": "2022-03-18T07:10:07.208Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-18T07:18:19.367Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-18T07:19:06.023Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-18T07:19:15.863Z"
   },
   {
    "duration": 18,
    "start_time": "2022-03-18T07:19:23.785Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-18T07:19:27.223Z"
   },
   {
    "duration": 17,
    "start_time": "2022-03-18T07:19:38.760Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T07:22:59.032Z"
   },
   {
    "duration": 22,
    "start_time": "2022-03-18T07:23:00.070Z"
   },
   {
    "duration": 2595,
    "start_time": "2022-03-18T07:24:56.246Z"
   },
   {
    "duration": 2701,
    "start_time": "2022-03-18T07:27:21.511Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T07:30:42.646Z"
   },
   {
    "duration": 2511,
    "start_time": "2022-03-18T07:30:43.509Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T07:30:48.151Z"
   },
   {
    "duration": 2656,
    "start_time": "2022-03-18T07:30:50.454Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T07:33:04.374Z"
   },
   {
    "duration": 2546,
    "start_time": "2022-03-18T07:33:06.597Z"
   },
   {
    "duration": 1770,
    "start_time": "2022-03-18T07:35:31.334Z"
   },
   {
    "duration": 390,
    "start_time": "2022-03-18T07:35:33.106Z"
   },
   {
    "duration": 27,
    "start_time": "2022-03-18T07:35:33.498Z"
   },
   {
    "duration": 134,
    "start_time": "2022-03-18T07:35:33.528Z"
   },
   {
    "duration": 139,
    "start_time": "2022-03-18T07:35:33.665Z"
   },
   {
    "duration": 324,
    "start_time": "2022-03-18T07:35:33.806Z"
   },
   {
    "duration": 318,
    "start_time": "2022-03-18T07:35:34.132Z"
   },
   {
    "duration": 421,
    "start_time": "2022-03-18T07:35:34.452Z"
   },
   {
    "duration": 463,
    "start_time": "2022-03-18T07:35:34.875Z"
   },
   {
    "duration": 192,
    "start_time": "2022-03-18T07:35:35.340Z"
   },
   {
    "duration": 184,
    "start_time": "2022-03-18T07:35:35.534Z"
   },
   {
    "duration": 176,
    "start_time": "2022-03-18T07:35:35.720Z"
   },
   {
    "duration": 29,
    "start_time": "2022-03-18T07:35:35.898Z"
   },
   {
    "duration": 121,
    "start_time": "2022-03-18T07:35:35.966Z"
   },
   {
    "duration": 189,
    "start_time": "2022-03-18T07:35:36.090Z"
   },
   {
    "duration": 182,
    "start_time": "2022-03-18T07:35:36.283Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-18T07:35:36.467Z"
   },
   {
    "duration": 118,
    "start_time": "2022-03-18T07:35:36.472Z"
   },
   {
    "duration": 431,
    "start_time": "2022-03-18T07:35:36.591Z"
   },
   {
    "duration": 13,
    "start_time": "2022-03-18T07:35:37.024Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T07:35:37.039Z"
   },
   {
    "duration": 34,
    "start_time": "2022-03-18T07:35:37.047Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-18T07:35:37.083Z"
   },
   {
    "duration": 2744,
    "start_time": "2022-03-18T07:35:37.090Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-18T07:35:39.836Z"
   },
   {
    "duration": 2707,
    "start_time": "2022-03-18T07:35:39.844Z"
   },
   {
    "duration": 1543,
    "start_time": "2022-03-30T04:59:50.671Z"
   },
   {
    "duration": 387,
    "start_time": "2022-03-30T04:59:52.216Z"
   },
   {
    "duration": 36,
    "start_time": "2022-03-30T04:59:52.605Z"
   },
   {
    "duration": 114,
    "start_time": "2022-03-30T04:59:52.643Z"
   },
   {
    "duration": 149,
    "start_time": "2022-03-30T04:59:52.759Z"
   },
   {
    "duration": 321,
    "start_time": "2022-03-30T04:59:52.909Z"
   },
   {
    "duration": 309,
    "start_time": "2022-03-30T04:59:53.233Z"
   },
   {
    "duration": 398,
    "start_time": "2022-03-30T04:59:53.543Z"
   },
   {
    "duration": 464,
    "start_time": "2022-03-30T04:59:53.943Z"
   },
   {
    "duration": 182,
    "start_time": "2022-03-30T04:59:54.410Z"
   },
   {
    "duration": 190,
    "start_time": "2022-03-30T04:59:54.594Z"
   },
   {
    "duration": 196,
    "start_time": "2022-03-30T04:59:54.786Z"
   },
   {
    "duration": 60,
    "start_time": "2022-03-30T04:59:54.984Z"
   },
   {
    "duration": 194,
    "start_time": "2022-03-30T04:59:55.046Z"
   },
   {
    "duration": 196,
    "start_time": "2022-03-30T04:59:55.243Z"
   },
   {
    "duration": 194,
    "start_time": "2022-03-30T04:59:55.442Z"
   },
   {
    "duration": 5,
    "start_time": "2022-03-30T04:59:55.639Z"
   },
   {
    "duration": 130,
    "start_time": "2022-03-30T04:59:55.646Z"
   },
   {
    "duration": 484,
    "start_time": "2022-03-30T04:59:55.778Z"
   },
   {
    "duration": 14,
    "start_time": "2022-03-30T04:59:56.264Z"
   },
   {
    "duration": 4,
    "start_time": "2022-03-30T04:59:56.280Z"
   },
   {
    "duration": 19,
    "start_time": "2022-03-30T04:59:56.285Z"
   },
   {
    "duration": 30,
    "start_time": "2022-03-30T04:59:56.306Z"
   },
   {
    "duration": 2430,
    "start_time": "2022-03-30T04:59:56.338Z"
   },
   {
    "duration": 6,
    "start_time": "2022-03-30T04:59:58.769Z"
   },
   {
    "duration": 2435,
    "start_time": "2022-03-30T04:59:58.776Z"
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
   "nav_menu": {},
   "number_sections": true,
   "sideBar": true,
   "skip_h1_title": true,
   "title_cell": "Table of Contents",
   "title_sidebar": "Contents",
   "toc_cell": false,
   "toc_position": {},
   "toc_section_display": true,
   "toc_window_display": false
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
