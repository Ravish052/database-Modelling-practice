# Discord DB design



we have 4 main entities 

users - > users using the app

servers ->  collection of channels, like communities

channels -> Channels exist inside servers

messages -> posts inside the channels



 USERS CAN JOIN MANY SERVERS AND EACH SERVER CAN HAVE MANY USERS --> this is a MANY - TO - MANY relationship. to handle this we create a table called server_member



CHANNEL >>

a channel is like an area where messages can be sent

and are often named around topics or areas to help organize the messages for the server.

each channel belong to one server and have a name and position for ordering. theres also a topic, which is like description of the channel.

type relates to channel_type lookup table, which has value slike text or voice



MESSAGES >>>

messages belong to a channel and are created by user. this table will grow very large, as every message is stored here. in a real system we need to partition it by channel or by time, and then use indices or sharding for performance.

a user can attach one or more files to a message like a screenshot or a video, A message can also have reactions



ROLES >>>

roles define what a user can do in a server. each server can have multiple roles such as administrator, or member, or whatever is defined for the server. also each member can have multiple roles on different servers so we add a roles table linked to servers, and a join table called server_member_role. we also have permissions, such as banning user, or adding new user. 







