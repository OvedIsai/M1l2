# M1l2

import discord
import random, os

from discord.ext import commands
intents = discord.Intents.default()
intents.message_content = True
bot = comands = commands.Bot(command_prefix= '!', intents=intents)

@bot.event
async def on_ready():
    print(f'consegos {bot.user}')

@bot.command()
async def consejo1(ctx):
    await ctx.send(f'puedes recojer la  basura de tu casa')

@bot.command()
async def consejo2(ctx):
    await ctx.send(f'no quemar basura es mejor enterrarla')

@bot.command()
async def consejo3(ctx):
    await ctx.send(f'no arrojar basura en la calle')

@bot.command()
async def consejo4(ctx):
    await ctx.send(f'no arrojar basura en los rios')

@bot.command()
async def consejo5(ctx):
    await ctx.send(f'no arrojar basura en los mares')

@bot.command()
async def consejo6(ctx):
    await ctx.send(f'no arrojar basura en los bosques')

@bot.command()
async def consejo7(ctx):
    await ctx.send(f'no arrojar basura en los parques')

@bot.command()
async def consejo8(ctx):
    await ctx.send(f'no arrojar basura en los campos')

@bot.command()
async def consejo9(ctx):
    await ctx.send(f'no arrojar basura en los desiertos')

@bot.command()
async def consejo10(ctx):
    await ctx.send(f'reciclar la basura para ayudar al medio ambiente')

bot.run('token')
