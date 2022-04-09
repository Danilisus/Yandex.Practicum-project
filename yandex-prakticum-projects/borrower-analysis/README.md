{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Исследование надёжности заёмщиков\n",
    "\n",
    "Заказчик — кредитный отдел банка. Нужно разобраться, влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. Входные данные от банка — статистика о платёжеспособности клиентов.\n",
    "\n",
    "Результаты исследования будут учтены при построении модели **кредитного скоринга**."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**План исследования**\n",
    "1. Открыть и изучить файл с данными.\n",
    "2. Предобратока данных:\n",
    "    * Обратотка пропусков;\n",
    "    * Замена типов данных;\n",
    "    * Обратотка дубликатов;\n",
    "    * Лемматизация;\n",
    "    * Категоризация данных;\n",
    "3. Провести исследование данных:\n",
    "    * Проверить наличие зависимости между ниличием детей и возвратом кредита;\n",
    "    * Проверить наличие зависимости между семейным положением и возвратом кредита в срок;\n",
    "    * Проверить наличие зависимости между уровнем дохода и возвратом кредита в срок;\n",
    "    * Определить влияние целей кредита на его возврат в срок.\n",
    "4. Общий вывод."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Общий вывод"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Таким образом мы провели анализ возврата кредита клиентам банка. Из данного анализа можно сделать следующие выводы: \n",
    "\n",
    "* чаще возвращают кредиты на ремонт; \n",
    "* люди с низким и высоким уровнем ежемесечного дохода; \n",
    "* также чаще возвращают кредит вдовы/вдовцы и семьи без детей."
   ]
  }
 ],
 "metadata": {
  "ExecuteTimeLog": [
   {
    "duration": 852,
    "start_time": "2021-12-13T06:10:32.351Z"
   },
   {
    "duration": 103,
    "start_time": "2021-12-13T06:37:03.639Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-13T08:39:19.188Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-13T08:39:36.837Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-13T08:43:33.667Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-13T08:43:56.932Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-13T12:07:43.050Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-13T12:08:03.728Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-13T12:09:23.277Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-13T12:10:51.235Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-13T12:19:38.156Z"
   },
   {
    "duration": 100,
    "start_time": "2021-12-13T12:21:14.973Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-13T12:21:18.972Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-13T12:23:55.852Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-13T12:24:25.579Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-13T12:25:05.884Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-13T12:25:46.619Z"
   },
   {
    "duration": 537,
    "start_time": "2021-12-13T12:26:11.515Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-13T12:26:19.356Z"
   },
   {
    "duration": 105,
    "start_time": "2021-12-14T06:36:41.208Z"
   },
   {
    "duration": 317,
    "start_time": "2021-12-14T06:36:53.040Z"
   },
   {
    "duration": 878,
    "start_time": "2021-12-14T06:37:40.395Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-14T06:38:54.443Z"
   },
   {
    "duration": 90,
    "start_time": "2021-12-14T06:59:02.702Z"
   },
   {
    "duration": 89,
    "start_time": "2021-12-14T06:59:10.471Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-14T07:11:19.270Z"
   },
   {
    "duration": 91,
    "start_time": "2021-12-14T07:27:56.844Z"
   },
   {
    "duration": -48,
    "start_time": "2021-12-14T07:28:18.231Z"
   },
   {
    "duration": 6402,
    "start_time": "2021-12-14T07:28:22.630Z"
   },
   {
    "duration": 6666,
    "start_time": "2021-12-14T07:29:04.324Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-14T07:34:28.812Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T07:34:38.314Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-14T07:36:27.332Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-14T07:37:53.355Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T07:39:10.356Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-14T08:31:49.664Z"
   },
   {
    "duration": 6881,
    "start_time": "2021-12-14T08:38:14.407Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-14T08:38:46.142Z"
   },
   {
    "duration": 6423,
    "start_time": "2021-12-14T08:40:01.920Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-14T08:40:30.356Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-14T08:41:03.567Z"
   },
   {
    "duration": 6507,
    "start_time": "2021-12-14T08:41:14.895Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-14T08:41:22.222Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-14T08:41:44.334Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-14T09:13:07.431Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-14T09:13:24.557Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T09:28:35.458Z"
   },
   {
    "duration": 366,
    "start_time": "2021-12-14T10:02:38.311Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-14T10:02:55.623Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-14T10:04:12.570Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-14T10:04:43.255Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T10:09:16.838Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-14T10:09:31.799Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T10:09:49.638Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-14T10:26:03.972Z"
   },
   {
    "duration": 244,
    "start_time": "2021-12-14T10:34:09.723Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-14T10:35:30.457Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-14T10:36:36.171Z"
   },
   {
    "duration": 292,
    "start_time": "2021-12-14T10:39:24.948Z"
   },
   {
    "duration": 275,
    "start_time": "2021-12-14T10:40:14.420Z"
   },
   {
    "duration": 316,
    "start_time": "2021-12-14T10:42:35.603Z"
   },
   {
    "duration": 244,
    "start_time": "2021-12-14T10:49:47.059Z"
   },
   {
    "duration": 231,
    "start_time": "2021-12-14T10:50:26.626Z"
   },
   {
    "duration": 254,
    "start_time": "2021-12-14T10:50:34.674Z"
   },
   {
    "duration": 312,
    "start_time": "2021-12-14T10:54:15.427Z"
   },
   {
    "duration": 249,
    "start_time": "2021-12-14T10:54:23.778Z"
   },
   {
    "duration": 241,
    "start_time": "2021-12-14T10:55:54.259Z"
   },
   {
    "duration": 317,
    "start_time": "2021-12-14T10:56:45.009Z"
   },
   {
    "duration": 338,
    "start_time": "2021-12-14T10:57:04.946Z"
   },
   {
    "duration": 96,
    "start_time": "2021-12-14T10:57:14.545Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-14T10:57:14.645Z"
   },
   {
    "duration": 72,
    "start_time": "2021-12-14T10:57:14.671Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T10:57:14.746Z"
   },
   {
    "duration": 65,
    "start_time": "2021-12-14T10:57:14.757Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-14T10:57:18.947Z"
   },
   {
    "duration": 4434,
    "start_time": "2021-12-14T10:58:17.425Z"
   },
   {
    "duration": 6022,
    "start_time": "2021-12-14T10:58:38.130Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-14T10:59:47.922Z"
   },
   {
    "duration": 38,
    "start_time": "2021-12-14T10:59:59.009Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-14T11:05:49.553Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-14T11:06:27.553Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-14T11:07:23.232Z"
   },
   {
    "duration": 256,
    "start_time": "2021-12-14T11:10:39.760Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T11:10:45.057Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T11:10:58.271Z"
   },
   {
    "duration": 92,
    "start_time": "2021-12-14T11:11:13.683Z"
   },
   {
    "duration": 39,
    "start_time": "2021-12-14T11:11:13.777Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-14T11:11:13.819Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-14T11:11:13.858Z"
   },
   {
    "duration": 67,
    "start_time": "2021-12-14T11:11:13.866Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-14T11:11:13.936Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T11:11:13.943Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-14T11:11:13.954Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T11:11:16.432Z"
   },
   {
    "duration": 276,
    "start_time": "2021-12-14T11:16:29.839Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T11:16:35.504Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T11:33:07.892Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-14T11:33:39.422Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T11:34:14.862Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-14T11:35:47.733Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-14T11:36:11.741Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-14T11:37:10.877Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-14T11:44:28.238Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-14T11:45:35.932Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T11:46:10.852Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T11:46:17.836Z"
   },
   {
    "duration": 85,
    "start_time": "2021-12-14T11:48:38.492Z"
   },
   {
    "duration": 267,
    "start_time": "2021-12-14T11:54:41.938Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T11:55:58.252Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-14T11:56:17.110Z"
   },
   {
    "duration": 2705,
    "start_time": "2021-12-14T11:56:30.412Z"
   },
   {
    "duration": 266,
    "start_time": "2021-12-14T11:57:38.026Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-14T12:25:11.230Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-14T12:25:28.118Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-14T12:25:37.821Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-14T12:25:44.391Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-14T12:25:52.031Z"
   },
   {
    "duration": 611,
    "start_time": "2021-12-15T05:49:17.806Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-15T05:49:18.418Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-15T05:49:18.433Z"
   },
   {
    "duration": 3,
    "start_time": "2021-12-15T05:49:18.452Z"
   },
   {
    "duration": 40,
    "start_time": "2021-12-15T05:49:18.456Z"
   },
   {
    "duration": 3,
    "start_time": "2021-12-15T05:49:18.497Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T05:49:18.502Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-15T05:49:18.511Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-15T05:49:18.533Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T05:50:08.831Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T05:57:10.264Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T05:59:48.793Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T06:00:15.160Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T06:00:25.544Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T06:01:01.095Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-15T06:04:19.401Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T06:04:26.664Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T06:04:35.704Z"
   },
   {
    "duration": 1066,
    "start_time": "2021-12-15T07:03:07.432Z"
   },
   {
    "duration": 6544,
    "start_time": "2021-12-15T07:09:19.448Z"
   },
   {
    "duration": 6088,
    "start_time": "2021-12-15T07:09:38.993Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:10:25.890Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T07:10:35.729Z"
   },
   {
    "duration": 239,
    "start_time": "2021-12-15T07:11:33.987Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-15T07:15:55.345Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T07:17:18.641Z"
   },
   {
    "duration": 2,
    "start_time": "2021-12-15T07:17:31.631Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T07:17:34.319Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:18:13.952Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T07:18:27.855Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:18:37.887Z"
   },
   {
    "duration": 916,
    "start_time": "2021-12-15T07:20:43.778Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-15T07:21:16.223Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-15T07:21:22.334Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-15T07:21:43.423Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-15T07:21:49.630Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-15T07:23:05.456Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-15T07:23:07.936Z"
   },
   {
    "duration": 267,
    "start_time": "2021-12-15T07:28:46.286Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-15T07:28:56.462Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-15T07:28:59.566Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T07:42:19.701Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:42:51.244Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:43:09.388Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T07:43:38.892Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:44:32.253Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:45:58.331Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T07:46:08.251Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-15T08:34:55.267Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T08:41:13.431Z"
   },
   {
    "duration": 250,
    "start_time": "2021-12-15T08:41:57.992Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-15T08:42:20.359Z"
   },
   {
    "duration": 406,
    "start_time": "2021-12-15T08:47:22.653Z"
   },
   {
    "duration": 419,
    "start_time": "2021-12-15T08:49:34.823Z"
   },
   {
    "duration": 247,
    "start_time": "2021-12-15T08:50:19.627Z"
   },
   {
    "duration": 241,
    "start_time": "2021-12-15T08:50:35.415Z"
   },
   {
    "duration": 6967,
    "start_time": "2021-12-15T08:50:54.630Z"
   },
   {
    "duration": 407,
    "start_time": "2021-12-15T08:51:10.104Z"
   },
   {
    "duration": 408,
    "start_time": "2021-12-15T08:51:24.326Z"
   },
   {
    "duration": 456,
    "start_time": "2021-12-15T08:51:48.822Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T08:54:30.213Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T08:54:36.966Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-15T08:54:48.133Z"
   },
   {
    "duration": 125,
    "start_time": "2021-12-15T08:54:56.789Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-15T08:54:59.868Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-15T08:59:14.380Z"
   },
   {
    "duration": 243,
    "start_time": "2021-12-15T10:31:52.944Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-15T10:32:07.160Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-15T10:32:13.400Z"
   },
   {
    "duration": 239,
    "start_time": "2021-12-15T10:39:38.062Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-15T10:39:52.759Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-15T10:39:59.575Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-15T11:02:47.046Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-15T11:14:09.858Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-15T12:19:10.566Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-15T12:19:41.480Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-15T12:20:03.239Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-15T12:20:11.768Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-15T12:20:17.496Z"
   },
   {
    "duration": 37,
    "start_time": "2021-12-15T12:26:42.121Z"
   },
   {
    "duration": 866,
    "start_time": "2021-12-15T16:38:31.262Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-15T16:38:32.130Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-15T16:38:32.156Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-15T16:38:32.187Z"
   },
   {
    "duration": 55,
    "start_time": "2021-12-15T16:38:32.194Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-15T16:38:32.251Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-15T16:38:32.259Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-15T16:38:32.270Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-15T16:38:32.303Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-15T16:38:32.324Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-15T16:38:32.352Z"
   },
   {
    "duration": 148,
    "start_time": "2021-12-15T16:38:32.373Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-15T16:38:32.525Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-15T16:38:32.557Z"
   },
   {
    "duration": 53,
    "start_time": "2021-12-15T16:38:52.864Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-15T17:44:51.847Z"
   },
   {
    "duration": 39,
    "start_time": "2021-12-15T17:45:38.484Z"
   },
   {
    "duration": 89,
    "start_time": "2021-12-15T17:45:51.774Z"
   },
   {
    "duration": 343,
    "start_time": "2021-12-15T18:06:41.718Z"
   },
   {
    "duration": 290,
    "start_time": "2021-12-15T18:07:16.870Z"
   },
   {
    "duration": 254,
    "start_time": "2021-12-16T05:04:10.312Z"
   },
   {
    "duration": 818,
    "start_time": "2021-12-16T05:04:18.665Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-16T05:04:19.485Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-16T05:04:19.511Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-16T05:04:19.544Z"
   },
   {
    "duration": 62,
    "start_time": "2021-12-16T05:04:19.551Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T05:04:19.615Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-16T05:04:19.621Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-16T05:04:19.630Z"
   },
   {
    "duration": 50,
    "start_time": "2021-12-16T05:04:19.661Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-16T05:04:19.713Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-16T05:04:19.720Z"
   },
   {
    "duration": 208,
    "start_time": "2021-12-16T05:04:19.731Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-16T05:04:19.940Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-16T05:04:19.963Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T05:04:24.087Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-16T05:04:39.312Z"
   },
   {
    "duration": 305,
    "start_time": "2021-12-16T06:02:47.064Z"
   },
   {
    "duration": 960,
    "start_time": "2021-12-16T06:02:53.769Z"
   },
   {
    "duration": 241,
    "start_time": "2021-12-16T06:03:05.225Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T06:03:29.983Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-16T06:04:06.184Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T06:04:33.752Z"
   },
   {
    "duration": 3337,
    "start_time": "2021-12-16T07:05:50.284Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-16T07:08:57.480Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-16T07:21:15.758Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-16T07:35:51.362Z"
   },
   {
    "duration": 3,
    "start_time": "2021-12-16T07:38:30.459Z"
   },
   {
    "duration": 277,
    "start_time": "2021-12-16T07:40:05.812Z"
   },
   {
    "duration": 334,
    "start_time": "2021-12-16T08:25:41.389Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T08:37:53.422Z"
   },
   {
    "duration": 266,
    "start_time": "2021-12-16T08:43:40.830Z"
   },
   {
    "duration": 4793,
    "start_time": "2021-12-16T08:44:16.095Z"
   },
   {
    "duration": 4899,
    "start_time": "2021-12-16T08:44:49.837Z"
   },
   {
    "duration": 381,
    "start_time": "2021-12-16T08:49:09.357Z"
   },
   {
    "duration": 193,
    "start_time": "2021-12-16T08:57:50.847Z"
   },
   {
    "duration": 202,
    "start_time": "2021-12-16T09:00:03.277Z"
   },
   {
    "duration": 258,
    "start_time": "2021-12-16T09:02:39.355Z"
   },
   {
    "duration": 272,
    "start_time": "2021-12-16T09:02:54.461Z"
   },
   {
    "duration": 318,
    "start_time": "2021-12-16T09:04:14.332Z"
   },
   {
    "duration": 249,
    "start_time": "2021-12-16T09:04:51.116Z"
   },
   {
    "duration": 258,
    "start_time": "2021-12-16T09:04:57.563Z"
   },
   {
    "duration": 4323,
    "start_time": "2021-12-16T09:09:30.052Z"
   },
   {
    "duration": 85,
    "start_time": "2021-12-16T09:10:02.731Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-16T09:10:58.987Z"
   },
   {
    "duration": 59,
    "start_time": "2021-12-16T09:11:46.195Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-16T09:12:21.817Z"
   },
   {
    "duration": 67,
    "start_time": "2021-12-16T09:12:31.902Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-16T09:12:31.971Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T09:12:31.995Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-16T09:12:32.016Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-16T09:12:32.027Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-16T09:12:32.057Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-16T09:12:32.069Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-16T09:12:32.091Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T09:12:32.124Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-16T09:12:32.142Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-16T09:12:32.148Z"
   },
   {
    "duration": 129,
    "start_time": "2021-12-16T09:12:32.178Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T09:12:32.309Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-16T09:12:32.325Z"
   },
   {
    "duration": 78,
    "start_time": "2021-12-16T09:12:32.337Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-16T09:12:32.417Z"
   },
   {
    "duration": 3612,
    "start_time": "2021-12-16T09:12:32.424Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-16T09:12:36.038Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-16T09:12:45.995Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-16T09:13:20.315Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-16T09:13:26.683Z"
   },
   {
    "duration": 54,
    "start_time": "2021-12-16T09:14:42.218Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T09:14:52.940Z"
   },
   {
    "duration": 37,
    "start_time": "2021-12-16T09:15:37.850Z"
   },
   {
    "duration": 62,
    "start_time": "2021-12-16T09:15:58.778Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-16T09:16:04.875Z"
   },
   {
    "duration": 68,
    "start_time": "2021-12-16T09:17:48.371Z"
   },
   {
    "duration": 52,
    "start_time": "2021-12-16T09:17:48.441Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T09:17:48.495Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T09:17:48.516Z"
   },
   {
    "duration": 37,
    "start_time": "2021-12-16T09:17:48.522Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T09:17:48.561Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-16T09:17:48.578Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-16T09:17:48.597Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T09:17:48.631Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-16T09:17:48.652Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-16T09:17:48.662Z"
   },
   {
    "duration": 131,
    "start_time": "2021-12-16T09:17:48.685Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T09:17:48.817Z"
   },
   {
    "duration": 39,
    "start_time": "2021-12-16T09:17:48.834Z"
   },
   {
    "duration": 51,
    "start_time": "2021-12-16T09:17:53.019Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T09:17:55.850Z"
   },
   {
    "duration": 64,
    "start_time": "2021-12-16T09:19:23.894Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-16T09:19:23.959Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-16T09:19:23.990Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T09:19:24.012Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-16T09:19:24.017Z"
   },
   {
    "duration": 3,
    "start_time": "2021-12-16T09:19:24.042Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-16T09:19:24.047Z"
   },
   {
    "duration": 48,
    "start_time": "2021-12-16T09:19:24.056Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T09:19:24.106Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-16T09:19:24.127Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-16T09:19:24.134Z"
   },
   {
    "duration": 140,
    "start_time": "2021-12-16T09:19:24.161Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T09:19:24.302Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-16T09:19:24.320Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-16T09:19:41.145Z"
   },
   {
    "duration": 50,
    "start_time": "2021-12-16T09:19:48.256Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T09:19:51.658Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-16T09:54:30.214Z"
   },
   {
    "duration": 46,
    "start_time": "2021-12-16T09:54:43.164Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-16T09:55:06.998Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-16T09:59:23.640Z"
   },
   {
    "duration": 3850,
    "start_time": "2021-12-16T09:59:26.549Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-16T09:59:40.565Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-16T09:59:43.861Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-16T10:35:45.089Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T10:36:28.145Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-16T10:37:08.902Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T10:40:35.394Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T10:40:51.330Z"
   },
   {
    "duration": 113,
    "start_time": "2021-12-16T10:41:04.450Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T10:41:10.709Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-16T10:41:29.267Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-16T10:46:08.657Z"
   },
   {
    "duration": 278,
    "start_time": "2021-12-16T10:49:22.140Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T10:49:33.504Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T10:50:43.840Z"
   },
   {
    "duration": 254,
    "start_time": "2021-12-16T10:56:30.354Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-16T10:56:40.576Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-16T10:57:03.295Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-16T10:57:32.208Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-16T10:58:26.960Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-16T11:02:03.119Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-16T11:04:54.927Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T11:08:29.253Z"
   },
   {
    "duration": 251,
    "start_time": "2021-12-16T11:08:37.310Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-16T11:08:42.674Z"
   },
   {
    "duration": 272,
    "start_time": "2021-12-16T11:08:58.063Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-16T11:09:05.423Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-16T11:10:06.895Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T11:10:31.662Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T11:10:43.262Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T11:10:46.912Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-16T11:11:48.066Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T11:11:54.258Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-16T11:13:01.489Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T11:19:03.854Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T11:19:27.437Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T11:19:57.166Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-16T11:20:03.278Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-16T11:27:44.942Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T11:29:32.334Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-16T11:36:22.205Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-16T11:39:17.952Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-16T11:39:59.148Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-16T11:40:52.652Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-16T11:42:22.989Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-16T11:46:13.628Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-16T11:46:51.179Z"
   },
   {
    "duration": 48,
    "start_time": "2021-12-16T11:47:59.563Z"
   },
   {
    "duration": 38,
    "start_time": "2021-12-16T11:48:11.067Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-16T11:48:35.035Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T11:50:12.251Z"
   },
   {
    "duration": 7470,
    "start_time": "2021-12-16T11:55:06.747Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-16T11:55:33.675Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-16T12:01:50.682Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-16T12:02:21.073Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-16T12:03:39.594Z"
   },
   {
    "duration": 50,
    "start_time": "2021-12-16T12:03:48.365Z"
   },
   {
    "duration": 674,
    "start_time": "2021-12-17T04:59:00.566Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-17T04:59:01.242Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-17T04:59:01.292Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T04:59:01.318Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-17T04:59:01.341Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T04:59:01.375Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-17T04:59:01.393Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-17T04:59:01.410Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-17T04:59:01.447Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T04:59:01.484Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T04:59:01.494Z"
   },
   {
    "duration": 141,
    "start_time": "2021-12-17T04:59:01.517Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-17T04:59:01.660Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-17T04:59:01.675Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-17T04:59:01.700Z"
   },
   {
    "duration": 40,
    "start_time": "2021-12-17T04:59:01.725Z"
   },
   {
    "duration": 42,
    "start_time": "2021-12-17T04:59:08.843Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-17T04:59:17.101Z"
   },
   {
    "duration": 65,
    "start_time": "2021-12-17T04:59:22.936Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-17T04:59:23.003Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-17T04:59:23.023Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-17T04:59:23.045Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-17T04:59:23.091Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-17T04:59:23.117Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-17T04:59:23.137Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-17T04:59:23.145Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-17T04:59:23.182Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-17T04:59:23.206Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-17T04:59:23.221Z"
   },
   {
    "duration": 132,
    "start_time": "2021-12-17T04:59:23.249Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-17T04:59:23.383Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-17T04:59:23.403Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-17T04:59:23.415Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-17T04:59:23.429Z"
   },
   {
    "duration": 68,
    "start_time": "2021-12-17T04:59:23.451Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-17T04:59:23.520Z"
   },
   {
    "duration": 3671,
    "start_time": "2021-12-17T04:59:23.527Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T04:59:27.200Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-17T04:59:27.210Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-17T04:59:27.231Z"
   },
   {
    "duration": 45,
    "start_time": "2021-12-17T04:59:27.246Z"
   },
   {
    "duration": 41,
    "start_time": "2021-12-17T04:59:27.294Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-17T04:59:27.337Z"
   },
   {
    "duration": 50,
    "start_time": "2021-12-17T04:59:27.349Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-17T04:59:27.401Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T04:59:27.425Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T04:59:27.448Z"
   },
   {
    "duration": 64,
    "start_time": "2021-12-17T06:20:25.519Z"
   },
   {
    "duration": 67,
    "start_time": "2021-12-17T06:20:52.604Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-17T06:20:52.673Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T06:20:52.697Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-17T06:20:52.720Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-17T06:20:52.725Z"
   },
   {
    "duration": 3,
    "start_time": "2021-12-17T06:20:52.755Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-17T06:20:52.760Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T06:20:52.796Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-17T06:20:52.818Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-17T06:20:52.839Z"
   },
   {
    "duration": 59,
    "start_time": "2021-12-17T06:20:56.146Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T06:21:58.859Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T06:22:13.828Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-17T06:22:54.203Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-17T06:23:18.731Z"
   },
   {
    "duration": 64,
    "start_time": "2021-12-17T06:24:13.324Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-17T06:24:32.175Z"
   },
   {
    "duration": 69,
    "start_time": "2021-12-17T06:24:47.675Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-17T06:25:02.156Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T06:25:10.989Z"
   },
   {
    "duration": 146,
    "start_time": "2021-12-17T06:25:39.083Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T06:25:42.874Z"
   },
   {
    "duration": 245,
    "start_time": "2021-12-17T06:28:15.850Z"
   },
   {
    "duration": 69,
    "start_time": "2021-12-17T06:28:21.469Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-17T06:28:21.540Z"
   },
   {
    "duration": 51,
    "start_time": "2021-12-17T06:28:21.560Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-17T06:28:21.613Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-17T06:28:21.621Z"
   },
   {
    "duration": 3,
    "start_time": "2021-12-17T06:28:21.651Z"
   },
   {
    "duration": 38,
    "start_time": "2021-12-17T06:28:21.656Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-17T06:28:21.697Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-17T06:28:21.720Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-17T06:28:21.741Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-17T06:28:21.749Z"
   },
   {
    "duration": 168,
    "start_time": "2021-12-17T06:28:21.757Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-17T06:28:21.926Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-17T06:28:21.943Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-17T06:28:21.955Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T06:28:21.992Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-17T06:28:22.015Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-17T06:28:22.052Z"
   },
   {
    "duration": 3650,
    "start_time": "2021-12-17T06:28:22.059Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-17T06:28:25.712Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T06:28:25.723Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-17T06:28:25.742Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-17T06:28:25.758Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-17T06:28:25.804Z"
   },
   {
    "duration": 44,
    "start_time": "2021-12-17T06:28:25.849Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-17T06:28:25.895Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T06:28:25.912Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T06:28:25.932Z"
   },
   {
    "duration": 6586,
    "start_time": "2021-12-17T06:28:25.951Z"
   },
   {
    "duration": 162,
    "start_time": "2021-12-17T06:29:00.251Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T06:32:50.810Z"
   },
   {
    "duration": 594,
    "start_time": "2021-12-17T06:34:03.230Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-17T10:08:13.376Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-17T10:13:48.161Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-17T10:13:51.374Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-17T10:13:59.965Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-17T10:14:29.134Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-17T10:14:32.031Z"
   },
   {
    "duration": 27,
    "start_time": "2021-12-17T10:14:48.496Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-17T10:14:56.734Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-17T10:15:05.453Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T10:15:44.831Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-17T10:20:18.925Z"
   },
   {
    "duration": 133,
    "start_time": "2021-12-17T10:20:27.900Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T10:20:30.172Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-17T10:24:06.796Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T10:24:30.509Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-17T10:24:37.645Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-17T10:24:41.021Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-17T10:26:08.375Z"
   },
   {
    "duration": 4088,
    "start_time": "2021-12-17T10:26:14.589Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-17T10:26:26.413Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T10:39:40.477Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-17T10:39:41.487Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-17T10:39:56.221Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-17T10:39:57.503Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-17T10:45:22.605Z"
   },
   {
    "duration": 27,
    "start_time": "2021-12-17T10:47:19.197Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-17T10:48:29.517Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-17T10:50:34.172Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T10:53:53.292Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-17T10:55:27.072Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T10:57:05.723Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T11:23:58.150Z"
   },
   {
    "duration": 255,
    "start_time": "2021-12-17T11:24:38.038Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T11:24:43.591Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-17T11:24:56.279Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-17T11:25:33.719Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-17T11:29:02.358Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-17T11:29:35.126Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-17T11:33:43.925Z"
   },
   {
    "duration": 98,
    "start_time": "2021-12-18T11:48:19.654Z"
   },
   {
    "duration": 86,
    "start_time": "2021-12-18T11:48:24.745Z"
   },
   {
    "duration": 870,
    "start_time": "2021-12-18T11:48:47.419Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-18T11:48:48.291Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T11:48:48.336Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T11:48:48.371Z"
   },
   {
    "duration": 76,
    "start_time": "2021-12-18T11:48:48.381Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-18T11:48:48.460Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-18T11:48:48.468Z"
   },
   {
    "duration": 72,
    "start_time": "2021-12-18T11:48:48.481Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T11:48:48.555Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T11:48:48.585Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-18T11:48:48.624Z"
   },
   {
    "duration": 224,
    "start_time": "2021-12-18T11:48:48.633Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T11:48:48.859Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-18T11:48:48.883Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-18T11:48:48.924Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T11:48:48.945Z"
   },
   {
    "duration": 70,
    "start_time": "2021-12-18T11:48:48.979Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T11:48:49.052Z"
   },
   {
    "duration": 4464,
    "start_time": "2021-12-18T11:48:49.064Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-18T11:48:53.532Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T11:48:53.544Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-18T11:48:53.568Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-18T11:48:53.587Z"
   },
   {
    "duration": 101,
    "start_time": "2021-12-18T11:48:53.632Z"
   },
   {
    "duration": -320,
    "start_time": "2021-12-18T11:48:54.055Z"
   },
   {
    "duration": -321,
    "start_time": "2021-12-18T11:48:54.058Z"
   },
   {
    "duration": -324,
    "start_time": "2021-12-18T11:48:54.062Z"
   },
   {
    "duration": -324,
    "start_time": "2021-12-18T11:48:54.064Z"
   },
   {
    "duration": -324,
    "start_time": "2021-12-18T11:48:54.066Z"
   },
   {
    "duration": -324,
    "start_time": "2021-12-18T11:48:54.067Z"
   },
   {
    "duration": -328,
    "start_time": "2021-12-18T11:48:54.073Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T11:50:47.217Z"
   },
   {
    "duration": 92,
    "start_time": "2021-12-18T11:50:53.831Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-18T11:50:53.925Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-18T11:50:53.954Z"
   },
   {
    "duration": 39,
    "start_time": "2021-12-18T11:50:53.987Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-18T11:50:54.029Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T11:50:54.065Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T11:50:54.072Z"
   },
   {
    "duration": 67,
    "start_time": "2021-12-18T11:50:54.082Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-18T11:50:54.152Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-18T11:50:54.183Z"
   },
   {
    "duration": 39,
    "start_time": "2021-12-18T11:50:54.193Z"
   },
   {
    "duration": 211,
    "start_time": "2021-12-18T11:50:54.234Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T11:50:54.447Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-18T11:50:54.469Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T11:50:56.865Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-18T11:51:00.250Z"
   },
   {
    "duration": 50,
    "start_time": "2021-12-18T11:51:03.369Z"
   },
   {
    "duration": 6633,
    "start_time": "2021-12-18T11:53:20.007Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T11:53:30.738Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-18T11:53:35.592Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T11:53:40.057Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T11:53:42.137Z"
   },
   {
    "duration": 83,
    "start_time": "2021-12-18T11:53:47.009Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-18T11:53:47.095Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-18T11:53:47.141Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-18T11:53:47.175Z"
   },
   {
    "duration": 68,
    "start_time": "2021-12-18T11:53:47.188Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-18T11:53:47.259Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-18T11:53:47.265Z"
   },
   {
    "duration": 57,
    "start_time": "2021-12-18T11:53:47.291Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-18T11:53:47.350Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-18T11:53:47.382Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-18T11:53:47.403Z"
   },
   {
    "duration": 216,
    "start_time": "2021-12-18T11:53:47.436Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T11:53:47.654Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-18T11:53:47.676Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T11:53:53.448Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-18T11:53:58.065Z"
   },
   {
    "duration": 49,
    "start_time": "2021-12-18T11:54:04.289Z"
   },
   {
    "duration": 52,
    "start_time": "2021-12-18T11:54:28.841Z"
   },
   {
    "duration": 55,
    "start_time": "2021-12-18T11:55:05.217Z"
   },
   {
    "duration": 54,
    "start_time": "2021-12-18T11:55:23.713Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-18T11:59:54.178Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T12:00:12.858Z"
   },
   {
    "duration": 49,
    "start_time": "2021-12-18T12:02:46.449Z"
   },
   {
    "duration": 42,
    "start_time": "2021-12-18T12:02:47.714Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T12:02:51.745Z"
   },
   {
    "duration": 73,
    "start_time": "2021-12-18T12:08:53.097Z"
   },
   {
    "duration": 34,
    "start_time": "2021-12-18T12:08:56.227Z"
   },
   {
    "duration": 90,
    "start_time": "2021-12-18T12:09:03.363Z"
   },
   {
    "duration": 68,
    "start_time": "2021-12-18T12:09:03.455Z"
   },
   {
    "duration": 38,
    "start_time": "2021-12-18T12:09:03.529Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-18T12:09:03.569Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-18T12:09:03.577Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T12:09:03.639Z"
   },
   {
    "duration": 8,
    "start_time": "2021-12-18T12:09:03.648Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-18T12:09:03.660Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T12:09:03.726Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T12:09:03.760Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T12:09:03.771Z"
   },
   {
    "duration": 264,
    "start_time": "2021-12-18T12:09:03.782Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T12:09:04.049Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-18T12:09:04.071Z"
   },
   {
    "duration": 77,
    "start_time": "2021-12-18T12:09:04.093Z"
   },
   {
    "duration": 61,
    "start_time": "2021-12-18T12:09:04.172Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T12:09:09.770Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T12:24:27.922Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-18T12:26:28.094Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-18T12:28:35.301Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-18T12:28:54.053Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T12:29:37.773Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-18T12:30:02.862Z"
   },
   {
    "duration": 62,
    "start_time": "2021-12-18T12:30:45.901Z"
   },
   {
    "duration": 108,
    "start_time": "2021-12-18T12:31:43.974Z"
   },
   {
    "duration": 110,
    "start_time": "2021-12-18T12:32:00.660Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-18T12:32:45.405Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T12:33:04.070Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-18T12:33:15.773Z"
   },
   {
    "duration": 95,
    "start_time": "2021-12-18T12:33:35.614Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-18T12:33:35.727Z"
   },
   {
    "duration": 77,
    "start_time": "2021-12-18T12:33:35.765Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T12:33:35.846Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-18T12:33:35.855Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T12:33:35.890Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T12:33:35.928Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T12:33:35.939Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-18T12:33:35.975Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-18T12:33:36.037Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-18T12:33:36.050Z"
   },
   {
    "duration": 358,
    "start_time": "2021-12-18T12:33:36.065Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-18T12:33:36.426Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-18T12:33:36.445Z"
   },
   {
    "duration": 79,
    "start_time": "2021-12-18T12:33:36.463Z"
   },
   {
    "duration": 45,
    "start_time": "2021-12-18T12:33:36.545Z"
   },
   {
    "duration": 94,
    "start_time": "2021-12-18T12:33:39.448Z"
   },
   {
    "duration": 340,
    "start_time": "2021-12-18T12:34:37.086Z"
   },
   {
    "duration": 358,
    "start_time": "2021-12-18T12:34:49.846Z"
   },
   {
    "duration": 344,
    "start_time": "2021-12-18T12:35:00.086Z"
   },
   {
    "duration": 316,
    "start_time": "2021-12-18T12:36:19.454Z"
   },
   {
    "duration": 343,
    "start_time": "2021-12-18T12:36:43.166Z"
   },
   {
    "duration": 64,
    "start_time": "2021-12-18T12:36:49.493Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-18T12:39:32.355Z"
   },
   {
    "duration": 15,
    "start_time": "2021-12-18T12:40:07.934Z"
   },
   {
    "duration": 88,
    "start_time": "2021-12-18T12:40:17.145Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-18T12:40:17.236Z"
   },
   {
    "duration": 72,
    "start_time": "2021-12-18T12:40:17.269Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T12:40:17.344Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-18T12:40:17.351Z"
   },
   {
    "duration": 35,
    "start_time": "2021-12-18T12:40:17.389Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T12:40:17.427Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-18T12:40:17.440Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-18T12:40:17.476Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T12:40:17.537Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-18T12:40:17.549Z"
   },
   {
    "duration": 234,
    "start_time": "2021-12-18T12:40:17.565Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-18T12:40:17.801Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-18T12:40:17.814Z"
   },
   {
    "duration": 55,
    "start_time": "2021-12-18T12:40:17.839Z"
   },
   {
    "duration": 52,
    "start_time": "2021-12-18T12:40:17.924Z"
   },
   {
    "duration": 107,
    "start_time": "2021-12-18T12:40:17.979Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T12:40:18.088Z"
   },
   {
    "duration": 4604,
    "start_time": "2021-12-18T12:40:18.097Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T12:40:22.704Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T12:40:22.728Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-18T12:40:22.752Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-18T12:40:22.771Z"
   },
   {
    "duration": 72,
    "start_time": "2021-12-18T12:40:22.784Z"
   },
   {
    "duration": 4,
    "start_time": "2021-12-18T12:40:22.859Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-18T12:40:22.866Z"
   },
   {
    "duration": 58,
    "start_time": "2021-12-18T12:40:22.885Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T12:41:22.575Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-18T12:41:34.768Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T12:41:56.590Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T12:42:50.478Z"
   },
   {
    "duration": 27,
    "start_time": "2021-12-18T12:43:14.942Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-18T12:43:39.743Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T12:43:49.958Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T12:44:02.126Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-18T12:44:17.150Z"
   },
   {
    "duration": 37,
    "start_time": "2021-12-18T17:24:59.815Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T17:25:37.873Z"
   },
   {
    "duration": 26,
    "start_time": "2021-12-18T17:27:02.617Z"
   },
   {
    "duration": 65,
    "start_time": "2021-12-18T17:27:05.801Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-18T17:31:25.418Z"
   },
   {
    "duration": 118,
    "start_time": "2021-12-18T17:43:26.275Z"
   },
   {
    "duration": 41,
    "start_time": "2021-12-18T17:43:26.396Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-18T17:43:26.440Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-18T17:43:26.476Z"
   },
   {
    "duration": 48,
    "start_time": "2021-12-18T17:43:26.502Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T17:43:26.553Z"
   },
   {
    "duration": 27,
    "start_time": "2021-12-18T17:43:26.560Z"
   },
   {
    "duration": 44,
    "start_time": "2021-12-18T17:43:26.590Z"
   },
   {
    "duration": 40,
    "start_time": "2021-12-18T17:43:26.637Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-18T17:43:26.679Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-18T17:43:26.691Z"
   },
   {
    "duration": 233,
    "start_time": "2021-12-18T17:43:26.712Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-18T17:43:26.947Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-18T17:43:26.962Z"
   },
   {
    "duration": 51,
    "start_time": "2021-12-18T17:43:31.682Z"
   },
   {
    "duration": 45,
    "start_time": "2021-12-18T17:43:33.010Z"
   },
   {
    "duration": 69,
    "start_time": "2021-12-18T17:43:36.106Z"
   },
   {
    "duration": 51,
    "start_time": "2021-12-18T17:45:49.867Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T17:45:54.538Z"
   },
   {
    "duration": 42,
    "start_time": "2021-12-18T17:46:01.674Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T17:46:18.187Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T17:46:21.362Z"
   },
   {
    "duration": 84,
    "start_time": "2021-12-18T17:46:24.877Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T17:46:24.964Z"
   },
   {
    "duration": 57,
    "start_time": "2021-12-18T17:46:24.995Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T17:46:25.055Z"
   },
   {
    "duration": 46,
    "start_time": "2021-12-18T17:46:25.062Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-18T17:46:25.123Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-18T17:46:25.131Z"
   },
   {
    "duration": 44,
    "start_time": "2021-12-18T17:46:25.152Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T17:46:25.198Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-18T17:46:25.237Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-18T17:46:25.250Z"
   },
   {
    "duration": 230,
    "start_time": "2021-12-18T17:46:25.269Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-18T17:46:25.501Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-18T17:46:25.515Z"
   },
   {
    "duration": 52,
    "start_time": "2021-12-18T17:46:25.560Z"
   },
   {
    "duration": 45,
    "start_time": "2021-12-18T17:46:25.615Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-18T17:46:25.663Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T17:46:29.218Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T17:50:49.842Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-18T17:54:24.676Z"
   },
   {
    "duration": 277,
    "start_time": "2021-12-18T17:54:37.265Z"
   },
   {
    "duration": 89,
    "start_time": "2021-12-18T17:54:44.967Z"
   },
   {
    "duration": 67,
    "start_time": "2021-12-18T17:54:45.058Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T17:54:45.128Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T17:54:45.163Z"
   },
   {
    "duration": 62,
    "start_time": "2021-12-18T17:54:45.174Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T17:54:45.238Z"
   },
   {
    "duration": 16,
    "start_time": "2021-12-18T17:54:45.246Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-18T17:54:45.267Z"
   },
   {
    "duration": 50,
    "start_time": "2021-12-18T17:54:45.303Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T17:54:45.355Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-18T17:54:45.367Z"
   },
   {
    "duration": 234,
    "start_time": "2021-12-18T17:54:45.386Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-18T17:54:45.623Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T17:54:45.637Z"
   },
   {
    "duration": 58,
    "start_time": "2021-12-18T17:54:45.668Z"
   },
   {
    "duration": 41,
    "start_time": "2021-12-18T17:54:45.728Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-18T17:54:45.772Z"
   },
   {
    "duration": 42,
    "start_time": "2021-12-18T17:54:45.798Z"
   },
   {
    "duration": 6,
    "start_time": "2021-12-18T17:54:45.843Z"
   },
   {
    "duration": 4795,
    "start_time": "2021-12-18T17:54:45.851Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-18T17:54:50.648Z"
   },
   {
    "duration": 43,
    "start_time": "2021-12-18T17:54:50.660Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-18T17:54:50.708Z"
   },
   {
    "duration": 10,
    "start_time": "2021-12-18T17:54:50.729Z"
   },
   {
    "duration": 131,
    "start_time": "2021-12-18T17:57:08.588Z"
   },
   {
    "duration": 29,
    "start_time": "2021-12-18T17:57:08.721Z"
   },
   {
    "duration": 72,
    "start_time": "2021-12-18T17:57:08.753Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T17:57:08.828Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T17:57:08.841Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T17:57:08.877Z"
   },
   {
    "duration": 40,
    "start_time": "2021-12-18T17:57:08.884Z"
   },
   {
    "duration": 32,
    "start_time": "2021-12-18T17:57:08.925Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T17:57:08.959Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T17:57:08.990Z"
   },
   {
    "duration": 9,
    "start_time": "2021-12-18T17:57:09.029Z"
   },
   {
    "duration": 224,
    "start_time": "2021-12-18T17:57:09.040Z"
   },
   {
    "duration": 11,
    "start_time": "2021-12-18T17:57:09.266Z"
   },
   {
    "duration": 17,
    "start_time": "2021-12-18T17:57:09.280Z"
   },
   {
    "duration": 70,
    "start_time": "2021-12-18T17:57:09.299Z"
   },
   {
    "duration": 60,
    "start_time": "2021-12-18T17:57:09.371Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T17:57:09.434Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T17:57:09.461Z"
   },
   {
    "duration": 7,
    "start_time": "2021-12-18T17:57:09.483Z"
   },
   {
    "duration": 4506,
    "start_time": "2021-12-18T17:57:09.528Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-18T17:57:14.038Z"
   },
   {
    "duration": 24,
    "start_time": "2021-12-18T17:57:14.054Z"
   },
   {
    "duration": 54,
    "start_time": "2021-12-18T17:57:14.081Z"
   },
   {
    "duration": 14,
    "start_time": "2021-12-18T17:57:14.138Z"
   },
   {
    "duration": 69534,
    "start_time": "2021-12-18T17:57:14.155Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-18T17:58:23.692Z"
   },
   {
    "duration": 46,
    "start_time": "2021-12-18T17:58:23.700Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-18T17:58:23.749Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T17:58:23.770Z"
   },
   {
    "duration": 52,
    "start_time": "2021-12-18T17:58:23.794Z"
   },
   {
    "duration": 36,
    "start_time": "2021-12-18T17:58:23.849Z"
   },
   {
    "duration": 64,
    "start_time": "2021-12-18T17:58:23.888Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T17:58:23.955Z"
   },
   {
    "duration": 33,
    "start_time": "2021-12-18T17:59:06.940Z"
   },
   {
    "duration": 31,
    "start_time": "2021-12-18T17:59:24.644Z"
   },
   {
    "duration": 295,
    "start_time": "2021-12-18T18:00:04.516Z"
   },
   {
    "duration": 28,
    "start_time": "2021-12-18T18:00:21.284Z"
   },
   {
    "duration": 18,
    "start_time": "2021-12-18T18:00:46.219Z"
   },
   {
    "duration": 19,
    "start_time": "2021-12-18T18:00:56.412Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T18:01:07.956Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T18:01:16.059Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T18:01:27.060Z"
   },
   {
    "duration": 30,
    "start_time": "2021-12-18T18:03:12.908Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T18:05:22.196Z"
   },
   {
    "duration": 332,
    "start_time": "2021-12-18T18:06:03.735Z"
   },
   {
    "duration": 293,
    "start_time": "2021-12-18T18:06:18.957Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-18T18:07:32.605Z"
   },
   {
    "duration": 22,
    "start_time": "2021-12-18T18:08:39.788Z"
   },
   {
    "duration": 23,
    "start_time": "2021-12-18T18:08:44.964Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T18:09:11.565Z"
   },
   {
    "duration": 27,
    "start_time": "2021-12-18T18:09:38.886Z"
   },
   {
    "duration": 25,
    "start_time": "2021-12-18T18:10:00.517Z"
   },
   {
    "duration": 20,
    "start_time": "2021-12-18T18:10:15.856Z"
   },
   {
    "duration": 21,
    "start_time": "2021-12-18T18:10:29.380Z"
   },
   {
    "duration": 318,
    "start_time": "2021-12-20T16:51:30.279Z"
   },
   {
    "duration": 917,
    "start_time": "2021-12-20T16:51:39.533Z"
   },
   {
    "duration": 41,
    "start_time": "2021-12-20T16:51:40.453Z"
   },
   {
    "duration": 148,
    "start_time": "2021-12-20T16:51:40.497Z"
   },
   {
    "duration": 157,
    "start_time": "2021-12-20T16:51:40.648Z"
   },
   {
    "duration": 183,
    "start_time": "2021-12-20T16:51:40.807Z"
   },
   {
    "duration": 132,
    "start_time": "2021-12-20T16:51:40.992Z"
   },
   {
    "duration": 155,
    "start_time": "2021-12-20T16:51:41.127Z"
   },
   {
    "duration": 281,
    "start_time": "2021-12-20T16:51:41.286Z"
   },
   {
    "duration": 196,
    "start_time": "2021-12-20T16:51:41.571Z"
   },
   {
    "duration": 134,
    "start_time": "2021-12-20T16:51:41.769Z"
   },
   {
    "duration": 173,
    "start_time": "2021-12-20T16:51:41.906Z"
   },
   {
    "duration": 450,
    "start_time": "2021-12-20T16:51:42.081Z"
   },
   {
    "duration": 12,
    "start_time": "2021-12-20T16:51:42.534Z"
   },
   {
    "duration": 159,
    "start_time": "2021-12-20T16:51:42.549Z"
   },
   {
    "duration": 209,
    "start_time": "2021-12-20T16:51:42.711Z"
   },
   {
    "duration": 180,
    "start_time": "2021-12-20T16:51:42.922Z"
   },
   {
    "duration": 151,
    "start_time": "2021-12-20T16:51:43.105Z"
   },
   {
    "duration": 131,
    "start_time": "2021-12-20T16:51:43.259Z"
   },
   {
    "duration": 133,
    "start_time": "2021-12-20T16:51:43.392Z"
   },
   {
    "duration": 5343,
    "start_time": "2021-12-20T16:51:43.527Z"
   },
   {
    "duration": 13,
    "start_time": "2021-12-20T16:51:48.873Z"
   },
   {
    "duration": 186,
    "start_time": "2021-12-20T16:51:48.889Z"
   },
   {
    "duration": 164,
    "start_time": "2021-12-20T16:51:49.082Z"
   },
   {
    "duration": 165,
    "start_time": "2021-12-20T16:51:49.249Z"
   },
   {
    "duration": 72787,
    "start_time": "2021-12-20T16:51:49.416Z"
   },
   {
    "duration": 5,
    "start_time": "2021-12-20T16:53:02.205Z"
   },
   {
    "duration": 282,
    "start_time": "2021-12-20T16:53:02.213Z"
   },
   {
    "duration": 262,
    "start_time": "2021-12-20T16:53:02.498Z"
   },
   {
    "duration": 263,
    "start_time": "2021-12-20T16:53:02.763Z"
   },
   {
    "duration": 262,
    "start_time": "2021-12-20T16:53:03.028Z"
   },
   {
    "duration": 350,
    "start_time": "2021-12-20T16:53:03.294Z"
   },
   {
    "duration": 190,
    "start_time": "2021-12-20T16:53:03.647Z"
   },
   {
    "duration": 169,
    "start_time": "2021-12-20T16:53:03.840Z"
   },
   {
    "duration": 454,
    "start_time": "2022-04-01T17:59:01.023Z"
   },
   {
    "duration": 139,
    "start_time": "2022-04-01T17:59:01.480Z"
   },
   {
    "duration": 77,
    "start_time": "2022-04-01T17:59:01.621Z"
   },
   {
    "duration": 30,
    "start_time": "2022-04-01T17:59:01.701Z"
   },
   {
    "duration": 6,
    "start_time": "2022-04-01T17:59:01.733Z"
   },
   {
    "duration": 63,
    "start_time": "2022-04-01T17:59:01.741Z"
   },
   {
    "duration": 5,
    "start_time": "2022-04-01T17:59:01.806Z"
   },
   {
    "duration": 18,
    "start_time": "2022-04-01T17:59:01.813Z"
   },
   {
    "duration": 37,
    "start_time": "2022-04-01T17:59:01.833Z"
   },
   {
    "duration": 32,
    "start_time": "2022-04-01T17:59:01.889Z"
   },
   {
    "duration": 10,
    "start_time": "2022-04-01T17:59:01.923Z"
   },
   {
    "duration": 13,
    "start_time": "2022-04-01T17:59:01.935Z"
   },
   {
    "duration": 151,
    "start_time": "2022-04-01T17:59:01.951Z"
   },
   {
    "duration": 15,
    "start_time": "2022-04-01T17:59:02.104Z"
   },
   {
    "duration": 22,
    "start_time": "2022-04-01T17:59:02.122Z"
   },
   {
    "duration": 88,
    "start_time": "2022-04-01T17:59:02.146Z"
   },
   {
    "duration": 54,
    "start_time": "2022-04-01T17:59:02.236Z"
   },
   {
    "duration": 29,
    "start_time": "2022-04-01T17:59:02.294Z"
   },
   {
    "duration": 24,
    "start_time": "2022-04-01T17:59:02.325Z"
   },
   {
    "duration": 32,
    "start_time": "2022-04-01T17:59:02.351Z"
   },
   {
    "duration": 4580,
    "start_time": "2022-04-01T17:59:02.386Z"
   },
   {
    "duration": 18,
    "start_time": "2022-04-01T17:59:06.969Z"
   },
   {
    "duration": 33,
    "start_time": "2022-04-01T17:59:06.989Z"
   },
   {
    "duration": 16,
    "start_time": "2022-04-01T17:59:07.024Z"
   },
   {
    "duration": 12,
    "start_time": "2022-04-01T17:59:07.042Z"
   },
   {
    "duration": 52504,
    "start_time": "2022-04-01T17:59:07.083Z"
   },
   {
    "duration": 3,
    "start_time": "2022-04-01T17:59:59.590Z"
   },
   {
    "duration": 30,
    "start_time": "2022-04-01T17:59:59.599Z"
   },
   {
    "duration": 14,
    "start_time": "2022-04-01T17:59:59.632Z"
   },
   {
    "duration": 49,
    "start_time": "2022-04-01T17:59:59.648Z"
   },
   {
    "duration": 21,
    "start_time": "2022-04-01T17:59:59.700Z"
   },
   {
    "duration": 24,
    "start_time": "2022-04-01T17:59:59.722Z"
   },
   {
    "duration": 51,
    "start_time": "2022-04-01T17:59:59.748Z"
   },
   {
    "duration": 25,
    "start_time": "2022-04-01T17:59:59.802Z"
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
   "version": "3.9.7"
  },
  "toc": {
   "base_numbering": 1,
   "nav_menu": {},
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
