# Echo-chambers
This repository contains data of a user reply network, built based on English language tweets related to Russian-Ukrainian war. This is the Russian-Ukrainian dataset used for the experiments in the paper to be cited, whic is mentioned below.

# Applications
This dataset can be used by the researchers involved in community detection and echo chamber detection in social networks to evaluate the communities detected by in their research work. It can be also used for other relevant research areas such as analysing  and simulating user behvaiour patternsand information propagation patterns of propagation of  in social networks.

# Data Files
(1) replyTweets_8-2022.csv - Contains data on reply tweets between users. Each row corresponds to a reply tweet and contains the userIDs of the sender and the receiver of the reply tweet.

(2) suspendUserReplies_8-2022.csv - Contains data on user interactions (reply tweets) with suspended users. 

(3) userReplies_8-2022.csv - Contains data on reply tweet counts between user pairs.

(4) userRepliesNoSelf_8-2022.csv - Contains data on reply tweet counts between user pairs after removing self replies (The users commenting to his/her own tweet).

# Data Fields
Following is the description of the data fields (column names) in the data files

(1) replyTweets_8-2022.csv

SourceUserID: Unique ID of the user who is the author of the parent tweet 
ReplyUserID: Unique ID of the user who is the author of the reply tweet 

(2) suspendUserReplies_8-2022.csv

UserID: Unique ID of the suspended user
NeighborCount: The number of users who have replied to the user's tweets and the number of users to whom the user has replied to

ReplyCount: The number of  users who have replied to the user's tweets and the number of users to whom the user has replied to  

AgreeCount: The number of agreeing replies sent to a user and received from a user

DisagreeCount: The number of disagreeing replies sent to a user and received from a user

SuspendCount: The number of suspended users who have replied to the user's tweets and the number of suspended users to whom the user has replied to 

SuspendReplies: The number of reply tweet the user has sent to a suspended user and the number of reply tweets the user has received from a suspended user

SuspendAgrees: The number of agreeing replies sent to a suspended user and received from a suspended user  

SuspendDisagrees: The number of disagreeing replies sent to a suspended user and received from a suspended user  

Stance: The stance of the user (U: Pro-Ukrainian, R:Pro-Russian, N: Neutral)

(3) userReplies_8-2022.csv

SourceUserID: UserID of the SourceUser  (SourceUser: The author of the parent tweets)

ReplyUserID: UserID of the ReplyUser (ReplyUser: The author of the reply tweets)

ReplyCount: The number of reply tweets sent by the ReplyUser to the parent tweets of the SourceUser

SourceStance: The stance of the SourceUser (U: Pro-Ukrainian, R:Pro-Russian, N: Neutral)

ReplyStance: The stance of the ReplyUser (U: Pro-Ukrainian, R:Pro-Russian, N: Neutral)

AgreeScore: The number of reply tweets sent by the ReplyUser to the parent tweets of SourceUser agreeing with the SourceUser (Number of occurrences where the parent and reply comment have the same stance)


(4) userRepliesNoSelf_8-2022.csv

SourceUserID: UserID of the SourceUser  (SourceUser: The author of the parent tweets)

ReplyUserID: UserID of the ReplyUser  (ReplyUser: The author of the reply tweets)

ReplyCount: The number of reply tweets sent by the ReplyUser to the parent tweets of the SourceUser

SourceStance: The stance of the SourceUser(U: Pro-Ukrainian, R:Pro-Russian, N: Neutral)

ReplyStance: The stance of the ReplyUser (U: Pro-Ukrainian, R:Pro-Russian, N: Neutral)

AgreeScore: The number of reply tweets sent by the ReplyUser to the parent tweets of SourceUser agreeing with the SourceUser (Number of occurrences where the parent and reply comment have the same stance)

# Paper citation
If you use any of the datasets, please cite the following paper.

Perera, Kushani, and Shanika Karunasekera. "Quantifying opinion rejection: A method to detect social media echo chambers." Pacific-Asia Conference on Knowledge Discovery and Data Mining. Singapore: Springer Nature Singapore, 2024.

@inproceedings{perera2024quantifying,
  title={Quantifying opinion rejection: A method to detect social media echo chambers},
  author={Perera, Kushani and Karunasekera, Shanika},
  booktitle={Pacific-Asia Conference on Knowledge Discovery and Data Mining},
  pages={57--69},
  year={2024},
  organization={Springer}
}
