import asyncio
from aiogram import Bot, Dispatcher, types
import os

TOKEN = os.getenv(8507545517:AAHV-vht_PHCRAJqxR73zBipdSn71GWALJo)

bot = Bot(8507545517:AAHV-vht_PHCRAJqxR73zBipdSn71GWALJo)
dp = Dispatcher()

@dp.message()
async def echo(message: types.Message):
    await message.answer("Бот запущен и работает!")

async def main():
    await dp.start_polling(bot)

if __name__ == "__main__":
    asyncio.run(main())
aiogram==3.4.1
worker: python bot.py
