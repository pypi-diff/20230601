# Comparing `tmp/Signal8-2.0.tar.gz` & `tmp/Signal8-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.0.tar", last modified: Tue May 30 22:42:50 2023, max compression
+gzip compressed data, was "Signal8-2.1.tar", last modified: Thu Jun  1 21:27:53 2023, max compression
```

## Comparing `Signal8-2.0.tar` & `Signal8-2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.324783 Signal8-2.0/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.0/LICENSE
--rw-rw-rw-   0        0        0     4356 2023-05-30 22:42:50.322956 Signal8-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3868 2023-05-22 23:14:08.000000 Signal8-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.242956 Signal8-2.0/Signal8/
--rw-rw-rw-   0        0        0     9975 2023-05-30 22:42:04.000000 Signal8-2.0/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.0/Signal8/__init__.py
--rw-rw-rw-   0        0        0      241 2023-05-30 22:27:03.000000 Signal8-2.0/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.314957 Signal8-2.0/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.0/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-05-30 18:28:08.000000 Signal8-2.0/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     4265 2023-05-30 17:26:10.000000 Signal8-2.0/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.0/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12606 2023-05-30 19:27:51.000000 Signal8-2.0/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-30 22:42:50.291960 Signal8-2.0/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4356 2023-05-30 22:42:49.000000 Signal8-2.0/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-30 22:42:50.000000 Signal8-2.0/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 22:42:49.000000 Signal8-2.0/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 22:42:49.000000 Signal8-2.0/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 22:42:50.324783 Signal8-2.0/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-30 22:42:22.000000 Signal8-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.739916 Signal8-2.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.1/LICENSE
+-rw-rw-rw-   0        0        0     4369 2023-06-01 21:27:53.737916 Signal8-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.602917 Signal8-2.1/Signal8/
+-rw-rw-rw-   0        0        0    10986 2023-06-01 21:26:04.000000 Signal8-2.1/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-2.1/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      226 2023-06-01 21:25:31.000000 Signal8-2.1/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.732920 Signal8-2.1/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.1/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-05-31 18:22:02.000000 Signal8-2.1/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-01 21:15:18.000000 Signal8-2.1/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     4265 2023-05-31 22:48:11.000000 Signal8-2.1/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.1/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12529 2023-06-01 21:21:33.000000 Signal8-2.1/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.1/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:27:53.707917 Signal8-2.1/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4369 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 21:27:53.000000 Signal8-2.1/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:27:53.740918 Signal8-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-01 21:27:15.000000 Signal8-2.1/setup.py
```

### Comparing `Signal8-2.0/LICENSE` & `Signal8-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.0/PKG-INFO` & `Signal8-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.0
+Version: 2.1
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -30,14 +30,15 @@
 ## Usage
 
 ```
 import Signal8
 
 env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
+env.close()
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `v_cluster` | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
```

### Comparing `Signal8-2.0/README.md` & `Signal8-2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ## Usage
 
 ```
 import Signal8
 
 env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
+env.close()
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `v_cluster` | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
```

### Comparing `Signal8-2.0/Signal8/Signal8.py` & `Signal8-2.1/Signal8/Signal8.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import time
 import copy
 import random
 import logging
 import threading
 import numpy as np
 
-from gymnasium.utils import EzPickle
+from .utils.npc import NPC
 from .utils.scenario import BaseScenario
 from .utils.core import Agent, Goal, Obstacle, World
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.problems import get_problem, get_problem_list
 
+from gymnasium.utils import EzPickle
+
 
 class raw_env(SimpleEnv, EzPickle):
-    def __init__(
-        self, 
-        num_agents=1,
-        render_mode="human"):
+    def __init__(self, num_agents=1, render_mode=None):
         
         scenario = Scenario()
         world = scenario.make_world(num_agents)
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
             max_cycles=500, 
-            continuous_actions=False,
         )
         
 env = make_env(raw_env)
 
 class Scenario(BaseScenario):
     def make_world(self, num_agents):
         world = World()
         self._add_logger()
         world.problem_scenarios = get_problem_list()
         
+        self.npc = []
         self.obstacle_locks = []
         self.scripted_obstacle_threads = []
         self.scripted_obstacle_running = False
 
         world.agents = [Agent() for _ in range(num_agents)]
         for i, agent in enumerate(world.agents):
             agent.name = f"agent_{i}"
             agent.collide = True
 
-        world.goals = [Goal() for _ in range(len(world.agents))]
+        # Agents has two goals (i.e., actual goal and start position)
+        # This is to ensure agent returns safely to start position
+        world.goals = [Goal() for _ in range(len(world.agents*2))]
         for i, goal in enumerate(world.goals):
             goal.name = f"goal_{i}"
             goal.collide = False
         
         # Minimum number of obstacles in a problem scenario 
         world.obstacles = [Obstacle() for _ in range(4)]
         for i, obstacle in enumerate(world.obstacles):
@@ -70,48 +71,50 @@
         world.dynamic_obstacle_constr = problem['dynamic_obs']
     
     """
     Returns goal constraints that haven't been selected to be used as an obstacle
     for the precision farming case (i.e., crop that wasn't selected as goal becomes an obstacle)
     """
     def _reset_agents_and_goals(self, world, np_random):
-        temp_start_constr = list(copy.copy(world.start_constr))
         temp_goal_constr = list(copy.copy(world.goal_constr))
         for i, agent in enumerate(world.agents):
-            agent.color = np.array([0, 0.8, 0])
+            agent.color = np.array([1, 0.95, 0.8])
             agent.state.p_vel = np.zeros(world.dim_p)
-            agent_constr = random.choice(temp_start_constr)
+            agent_constr = random.choice(world.start_constr)
             agent.state.p_pos = np_random.uniform(*zip(*agent_constr))
-            agent.start_pos = copy.copy(agent.state.p_pos)
-            temp_start_constr.remove(agent_constr)
 
-            agent.goal = world.goals[i]
-            agent.goal.color = np.array([0, 0, 0.8])
-            agent.goal.state.p_vel = np.zeros(world.dim_p)
+            agent.goal_a = world.goals[i]
+            agent.goal_a.color = np.array([0.835, 0.90, 0.831])
+            agent.goal_a.state.p_vel = np.zeros(world.dim_p)
             goal_constr = random.choice(temp_goal_constr)
-            agent.goal.state.p_pos = np_random.uniform(*zip(*goal_constr))
-            temp_goal_constr.remove(goal_constr)
+            agent.goal_a.state.p_pos = np_random.uniform(*zip(*goal_constr))
+            if world.problem_name.startswith('precision_farming'):
+                temp_goal_constr.remove(goal_constr)
+            
+            agent.goal_b = world.goals[len(world.goals) - 1 - i]
+            agent.goal_b.color = np.array([0.85, 0.90, 0.99])
+            agent.goal_b.state.p_vel = np.zeros(world.dim_p)
+            agent.goal_b.state.p_pos = copy.copy(agent.state.p_pos)
 
         return temp_goal_constr
     
     # Reset position of dynamic obstacles
     def _reset_dynamic_obstacle(self, world, obstacle, np_random, temp_dynamic_obs_constr):
         obstacle.size = 0.025
         obstacle.movable = True
         self.obstacle_locks += [threading.Lock()]
-        obstacle.color = np.array([0.5, 0, 0])
+        obstacle.color = np.array([0.26, 0.32, 0.36])
         obstacle.state.p_vel = np.zeros(world.dim_p)
         dynamic_obs_constr = random.choice(temp_dynamic_obs_constr)
         obstacle.state.p_pos = np_random.uniform(*zip(*dynamic_obs_constr))
-        obstacle.action_callback = self.action_callback
         temp_dynamic_obs_constr.remove(dynamic_obs_constr)
 
     # Reset position of static obstacles, taking leftover entities from goal constraints
     def _reset_static_obstacle(self, world, obstacle, np_random, temp_static_obs_constr):
-        obstacle.color = np.array([0.2, 0.2, 0.2])
+        obstacle.color = np.array([0.97, 0.801, 0.8])
         obstacle.state.p_vel = np.zeros(world.dim_p)
         static_obs_constr = random.choice(temp_static_obs_constr)
         obstacle.state.p_pos = np_random.uniform(*zip(*static_obs_constr))  
         temp_static_obs_constr.remove(static_obs_constr)
     
     # Add or remove obstacles to match the number of obstacles in problem scenario
     def _match_obstacles_to_problem(self, world, num_static):
@@ -125,104 +128,110 @@
     
     # Reset position of obstacles
     def _reset_obstacles(self, world, np_random, leftover_entities):
         temp_static_obs_constr = list(copy.copy(world.static_obstacle_constr))
         temp_static_obs_constr += leftover_entities
         temp_dynamic_obs_constr = list(copy.copy(world.dynamic_obstacle_constr))
         
-        num_dynamic_obs = len(temp_dynamic_obs_constr)
-        self.prev_action = {i: np.zeros(world.dim_p) for i in range(num_dynamic_obs)}
-        
+        num_dynamic_obs = len(temp_dynamic_obs_constr)        
         self._match_obstacles_to_problem(world, len(temp_static_obs_constr))
 
         for i, obstacle in enumerate(world.obstacles):
             if i < num_dynamic_obs:
                 self._reset_dynamic_obstacle(world, obstacle, np_random, temp_dynamic_obs_constr)
+                self.npc += [NPC(obstacle.state.p_pos)]
             else:
                 self._reset_static_obstacle(world, obstacle, np_random, temp_static_obs_constr)
     
     # Start a thread for each dynamic obstacle
     def _start_scripted_obstacles(self, world):
         idx = 0
         self.scripted_obstacle_running = True
         for obstacle in world.obstacles:
             if obstacle.movable:
                 t = threading.Thread(target=self.run_scripted_obstacle, args=(world, obstacle, idx))
                 t.start()
                 self.scripted_obstacle_threads.append(t)   
                 idx += 1
-    
-    # Reset entities in world
+                
     def reset_world(self, world, np_random, problem_name=None):
-        self._stop_scripted_obstacles()
+        self.npc.clear()
+        self.stop_scripted_obstacles()
         self._set_problem_scenario(world, np_random, problem_name)
         leftover_entities = self._reset_agents_and_goals(world, np_random)
         self._reset_obstacles(world, np_random, leftover_entities)
-        self._start_scripted_obstacles(world)
+        if problem_name is not None:
+            self._start_scripted_obstacles(world)
     
-    # Do not need to implement this function
+    # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
-
-    def observation(self, agent, world):
-        return np.concatenate((agent.state.p_pos, agent.state.p_vel))
     
+    def observation(self, agent, world):
+        agent_pos = agent.state.p_pos
+        agent_vel = agent.state.p_vel
+        
+        num_obstacles = len(world.obstacles)
+        max_observable_dist = agent.max_observable_dist
+        
+        observed_obstacles = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_obstacles)]
+        observed_goal = np.full_like(agent_pos, max_observable_dist)
+        
+        for i, obstacle in enumerate(world.obstacles):
+            if obstacle.movable:
+                with self.obstacle_locks[i]:
+                    obs_pos = obstacle.state.p_pos
+            else:
+                obs_pos = obstacle.state.p_pos
+            relative_pos = obs_pos - agent_pos
+            dist = np.linalg.norm(relative_pos)
+            if dist <= max_observable_dist:
+                observed_obstacles[i] = relative_pos
+                
+        goal_pos = agent.goal_b.state.p_pos if agent.reached_goal else agent.goal_a.state.p_pos
+        relative_goal_pos = goal_pos - agent_pos
+        goal_dist = np.linalg.norm(relative_goal_pos)
+        if goal_dist <= max_observable_dist:
+            observed_goal = relative_goal_pos
+        
+        return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
+            
     # Run a thread for each scripted obstacle
     def run_scripted_obstacle(self, world, obstacle, obstacle_idx):
-        sensitivity = 5.0
+        sensitivity = 2.0
         while self.scripted_obstacle_running:
             with self.obstacle_locks[obstacle_idx]:
-                self.logger.debug(f'{obstacle.name} started at size: {obstacle.size}, position: {obstacle.state.p_pos}')
-                action = self.action_callback(obstacle, world)
+                # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
+                action = self._action_callback(obstacle, world)
                 obstacle.action = action * sensitivity
                 obstacle.move()
-                self.logger.debug(f'{obstacle.name} is now: {obstacle.size}, position: {obstacle.state.p_pos}')
-                time.sleep(0.1)
+                time.sleep(0.25)
         
-    """
-    Disaster Response: Increase size of obstacle to resemble increasing size of fire/flood
-    Precision Farming: Move obstacle in a zamboni pattern to resemble the tractor
-    """
-    def action_callback(self, obs, world):
+    # disaster response: increase obstacle size to resemble increasing size of fire
+    # precision farming: move obstacle in a zig-zag pattern to resemble a tractor
+    def _action_callback(self, obs, world):
         action = np.zeros(world.dim_p)
-        
         problem_name = world.problem_name
-        problem_name = 'precision_farming_0'
         if problem_name == 'disaster_response_0':
-            obs.size *= 1.125
+            obs.size += 0.005
         elif problem_name == 'disaster_response_1':
-            obs.size *= 1.100
+            obs.size += 0.0075
         elif problem_name == 'disaster_response_2':
-            obs.size *= 1.150
+            obs.size += 0.01
         elif problem_name == 'disaster_response_3':
-            obs.size *= 1.050
+            obs.size += 0.0125
         elif problem_name.startswith('precision_farming'):
+            obs_num = int(problem_name.split('_')[-1])
             scenario_num = int(problem_name.split('_')[-1])
-            action = self._get_scripted_action(obs, scenario_num)
+            action = self.npc[obs_num].get_scripted_action(obs, scenario_num)
 
         return action
-    
-    def _get_scripted_action(self, obs, scenario):
-        obs_num = int(obs.name.split('_')[-1])
-        action = [+1, 0]
-        
-        if scenario == 0:
-            a=3
-        elif scenario == 1:
-            a=3
-        elif scenario == 2:
-            a=3
-        else:
-            a=3
-        
-        self.prev_action[obs_num] = action
-        return action
 
     # Stop all threads for scripted obstacles
-    def _stop_scripted_obstacles(self):
+    def stop_scripted_obstacles(self):
         self.scripted_obstacle_running = False
         for t in self.scripted_obstacle_threads:
             t.join()
         self.scripted_obstacle_threads.clear()
         self.obstacle_locks.clear()
         
     # Create a logger to log information from threads
```

### Comparing `Signal8-2.0/Signal8/utils/core.py` & `Signal8-2.1/Signal8/utils/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,23 +60,25 @@
 
 class Agent(Entity):  # properties of agent entities
     def __init__(self):
         super().__init__()
         # agents are movable by default
         self.movable = True
         # reached goal state
+        self.goal_a = None
         self.reached_goal = False
         # reached start state after reaching goal
+        self.goal_b = None
         self.returned_to_safety = False
-        # starting physical position
-        self.start_pos = None
         # state
         self.state = AgentState()
         # action
         self.action = None
+        # how far the agent can see
+        self.max_observable_dist = 0.30
 
 class World:  # multi-agent world
     def __init__(self):
         # list of agents and entities (can change at execution-time!)
         self.agents = []
         self.goals = []
         self.obstacles = []
```

### Comparing `Signal8-2.0/Signal8/utils/problems.py` & `Signal8-2.1/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.0/Signal8/utils/simple_env.py` & `Signal8-2.1/Signal8/utils/simple_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import gymnasium
 import numpy as np
 import pygame
 from gymnasium import spaces
 from gymnasium.utils import seeding
 
 from pettingzoo import AECEnv
-from pettingzoo.mpe._mpe_utils.core import Agent
 from pettingzoo.utils import wrappers
 from pettingzoo.utils.agent_selector import agent_selector
 
 def make_env(raw_env):
     def env(**kwargs):
         env = raw_env(**kwargs)
-        if env.continuous_actions:
-            env = wrappers.ClipOutOfBoundsWrapper(env)
-        else:
-            env = wrappers.AssertOutOfBoundsWrapper(env)
+        env = wrappers.AssertOutOfBoundsWrapper(env)
         env = wrappers.OrderEnforcingWrapper(env)
         return env
-
     return env
 
 
 class SimpleEnv(AECEnv):
     metadata = {
         "render_modes": ["human", "rgb_array"],
         "is_parallelizable": True,
@@ -31,37 +26,34 @@
 
     def __init__(
         self,
         scenario,
         world,
         max_cycles,
         render_mode=None,
-        continuous_actions=False,
         local_ratio=None,
     ):
         super().__init__()
 
         self.render_mode = render_mode
         pygame.init()
         self.viewer = None
         self.width = 700
         self.height = 700
         self.screen = pygame.Surface([self.width, self.height])
         self.max_size = 1
         self.game_font = pygame.freetype.Font(None, 20)
 
-        # Set up the drawing window
-
         self.renderOn = False
+        self._reset_called = False
         self.seed()
 
         self.max_cycles = max_cycles
         self.scenario = scenario
         self.world = world
-        self.continuous_actions = continuous_actions
         self.local_ratio = local_ratio
 
         self.scenario.reset_world(self.world, self.np_random)
         self.agents = [agent.name for agent in self.world.agents]
         self.possible_agents = self.agents[:]
         self._index_map = {agent.name: idx for idx, agent in enumerate(self.world.agents)}
 
@@ -70,27 +62,20 @@
         # set spaces
         self.action_spaces = dict()
         self.observation_spaces = dict()
         state_dim = 0
         for agent in self.world.agents:
             if agent.movable:
                 space_dim = self.world.dim_p * 2 + 1
-            elif self.continuous_actions:
-                space_dim = 0
             else:
                 space_dim = 1
 
             obs_dim = len(self.scenario.observation(agent, self.world))
             state_dim += obs_dim
-            if self.continuous_actions:
-                self.action_spaces[agent.name] = spaces.Box(
-                    low=0, high=1, shape=(space_dim,)
-                )
-            else:
-                self.action_spaces[agent.name] = spaces.Discrete(space_dim)
+            self.action_spaces[agent.name] = spaces.Discrete(space_dim)
             self.observation_spaces[agent.name] = spaces.Box(
                 low=-np.float32(1),
                 high=+np.float32(1),
                 shape=(obs_dim,),
                 dtype=np.float32,
             )
 
@@ -127,47 +112,63 @@
             for agent in self.possible_agents
         )
         return np.concatenate(states, axis=None)
 
     def reset(self, seed=None, return_info=False, options=None):        
         if seed is not None:
             self.seed(seed=seed)
-            
+        
         problem_scenario = options['problem_name']
         self.scenario.reset_world(self.world, self.np_random, problem_scenario)
 
         self.agents = self.possible_agents[:]
+        # PettingZoo Gymansium requires rewards to be set
+        # even if they are not used
         self.rewards = {name: 0.0 for name in self.agents}
         self._cumulative_rewards = {name: 0.0 for name in self.agents}
         self.terminations = {name: False for name in self.agents}
         self.truncations = {name: False for name in self.agents}
         self.infos = {name: {} for name in self.agents}
-
+        
+        self._reset_called = True
         self.agent_selection = self._agent_selector.reset()
         self.steps = 0
 
         self.current_actions = [None] * len(self.world.agents)
-
+        
+    def get_start_state(self):
+        if not self._reset_called:
+            raise Exception("Cannot get start state without calling reset() first")
+        
+        agent_pos = np.array([agent.state.p_pos for agent in self.world.agents])
+        goal_pos = np.array([(agent.goal_a.state.p_pos, agent.goal_b.state.p_pos) for agent in self.world.agents])
+        try:
+            [self.scenario.obstacle_locks[i].acquire() for i in range(len(self.scenario.obstacle_locks))]
+            obs_pos = np.array([obs.state.p_pos for obs in self.world.obstacles])
+        finally:
+            [self.scenario.obstacle_locks[i].release() for i in range(len(self.scenario.obstacle_locks))]
+        
+        entities = {'agents': agent_pos, 'goals': goal_pos, 'obstacles': obs_pos}
+        return entities
+        
     def _execute_world_step(self):
         # set action for each agent
         for i, agent in enumerate(self.world.agents):
             action = self.current_actions[i]
             scenario_action = []
             if agent.movable:
                 mdim = self.world.dim_p * 2 + 1
-                if self.continuous_actions:
-                    scenario_action.append(action[0:mdim])
-                    action = action[mdim:]
-                else:
-                    scenario_action.append(action % mdim)
-                    action //= mdim
-            self._set_action(scenario_action, agent, self.action_spaces[agent.name])
+                scenario_action.append(action % mdim)
+                action //= mdim
+            self._set_action(scenario_action, agent)
 
         self.world.step()
 
+        # PettingZoo Gymansium requires rewards to be set
+        # even if they are not used
         global_reward = 0.0
         if self.local_ratio is not None:
             global_reward = float(self.scenario.global_reward(self.world))
 
         for agent in self.world.agents:
             agent_reward = float(self.scenario.reward(agent, self.world))
             if self.local_ratio is not None:
@@ -177,78 +178,76 @@
                 )
             else:
                 reward = agent_reward
 
             self.rewards[agent.name] = reward
 
     # set env action for a particular agent
-    def _set_action(self, action, agent, action_space, time=None):
+    def _set_action(self, action, agent):
         if agent.movable:
             # physical action
             agent.action = np.zeros(self.world.dim_p)
-            if self.continuous_actions:
-                # Process continuous action as in OpenAI MPE
-                agent.action[0] += action[0][1] - action[0][2]
-                agent.action[1] += action[0][3] - action[0][4]
-            else:
-                # process discrete action
-                if action[0] == 1:
-                    agent.action[0] = -1.0
-                elif action[0] == 2:
-                    agent.action[0] = +1.0
-                elif action[0] == 3:
-                    agent.action[1] = -1.0
-                elif action[0] == 4:
-                    agent.action[1] = +1.0
-            sensitivity = 5.0
+            if action[0] == 1:
+                agent.action[0] = -1.0
+            elif action[0] == 2:
+                agent.action[0] = +1.0
+            elif action[0] == 3:
+                agent.action[1] = -1.0
+            elif action[0] == 4:
+                agent.action[1] = +1.0
+            sensitivity = 2.0
             agent.action *= sensitivity
             action = action[1:]
         # make sure we used all elements of action
         assert len(action) == 0
     
     # Check if episode is terminated or truncated
     def _episode_status(self):        
         dynamic_obs = [obs for obs in self.world.obstacles if obs.movable]
         static_obs = [obs for obs in self.world.obstacles if not obs.movable]
-    
-        goal_dist_threshold = self.world.agents[0].size + self.world.agents[0].goal.size
+
+        goal_dist_threshold = self.world.agents[0].size + self.world.agents[0].goal_a.size
         static_obs_threshold = self.world.agents[0].size + static_obs[0].size
-        
-        goal_dist = [np.linalg.norm(agent.state.p_pos - agent.goal.state.p_pos) for agent in self.world.agents]
+
+        goal_a_dist = [np.linalg.norm(agent.state.p_pos - agent.goal_a.state.p_pos) for agent in self.world.agents]
+        goal_b_dist = [np.linalg.norm(agent.state.p_pos - agent.goal_b.state.p_pos) for agent in self.world.agents]
         static_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in static_obs)
                            for agent in self.world.agents]
-        
+
         crossed_threshold_static = [dist <= static_obs_threshold for dist in static_obs_dist]
-        
+
+        for lock in self.scenario.obstacle_locks:
+            lock.acquire()
+
         try:
-            for i in range(len(dynamic_obs)):
-                self.scenario.obstacle_locks[i].acquire()
-                dynamic_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in dynamic_obs)
-                                    for agent in self.world.agents] 
-                dynamic_obs_threshold = [agent.size + obs.size for agent, obs in zip(self.world.agents, dynamic_obs)]   
-            
+            dynamic_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in dynamic_obs)
+                                for agent in self.world.agents] 
+            dynamic_obs_threshold = [agent.size + obs.size for agent, obs in zip(self.world.agents, dynamic_obs)]   
+
             crossed_threshold_dynamic = [dist <= threshold for dist, threshold in zip(dynamic_obs_dist, dynamic_obs_threshold)]
-                        
+
             truncations = [crossed_stat or crossed_dyn for crossed_stat, crossed_dyn in zip(crossed_threshold_static, crossed_threshold_dynamic)]
             truncations = [True] * self.num_agents if self.steps >= self.max_cycles else truncations
-            
+
             terminations = [False] * self.num_agents
-            for i, dist in enumerate(goal_dist):
+            for i, dist in enumerate(goal_a_dist):
                 if dist <= goal_dist_threshold:
-                    self.agents[i].reached_goal = True
-            
-            for i, agent in enumerate(self.world.agents):
-                if agent.reached_goal:
-                    dist_to_start = np.linalg.norm(agent.state.p_pos - agent.start_pos)
-                    start_dist_threshold = self.world.agents[0].size * 2
-                    if dist_to_start <= start_dist_threshold:
+                    self.world.agents[i].reached_goal = True
+
+            for i, dist in enumerate(goal_b_dist):
+                if self.world.agents[i].reached_goal:
+                    if dist <= goal_dist_threshold:
+                        self.agents[i].reached_safety = True
                         terminations[i] = True
         finally:
-            [self.scenario.obstacle_locks[i].release() for i, _ in enumerate(dynamic_obs)]
-            return {'terminations': terminations, 'truncations': truncations}
+            for lock in self.scenario.obstacle_locks:
+                lock.release()
+
+        return {'terminations': terminations, 'truncations': truncations}
+
 
     def step(self, action):
         if (
             self.terminations[self.agent_selection]
             or self.truncations[self.agent_selection]
         ):
             self._was_dead_step(action)
@@ -325,8 +324,9 @@
                 0 < x < self.width and 0 < y < self.height
             ), f"Coordinates {(x, y)} are out of bounds."
 
     def close(self):
         if self.renderOn:
             pygame.event.pump()
             pygame.display.quit()
-            self.renderOn = False
+            self.renderOn = False
+        self.unwrapped.scenario.stop_scripted_obstacles()
```

### Comparing `Signal8-2.0/Signal8.egg-info/PKG-INFO` & `Signal8-2.1/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.0
+Version: 2.1
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -30,14 +30,15 @@
 ## Usage
 
 ```
 import Signal8
 
 env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
+env.close()
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
 | :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `v_cluster` | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
```

### Comparing `Signal8-2.0/setup.py` & `Signal8-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.0",
+    version="2.1",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

