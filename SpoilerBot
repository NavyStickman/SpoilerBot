import discord
import random
import os
from discord.ext import commands, tasks

intents = discord.Intents(messages = True, guilds = True, reactions = True, members = True, presences = True)
client = commands.Bot(command_prefix = '.', intents = intents)

@client.event
async def on_ready():
  print("Ready")

#This is the spoiler wall command
@client.command()
async def spoilerWall(ctx):
  for i in range(50):
    await ctx.send(f"Spoiler Wall Message \n**|** *({i+1}/50 messages sent)*")

client.run("TOKEN")
