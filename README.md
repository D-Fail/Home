
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unique Social Media Design</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #121212; /* Dark background */
            color: #ffffff; /* White text */
        }

        /* Header */
        .header {
            background-color: #0D0D0D;
            padding: 15px;
            display: flex;
            justify-content: space-around;
            align-items: center;
            border-bottom: 2px solid #ffffff; /* White border */
        }

        .header button {
            background-color: #292929;
            color: #ffffff;
            border: none;
            border-radius: 5px;
            padding: 8px 10px;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s, transform 0.3s;
            width: 80px; /* Equal width for buttons */
        }

        .header button:hover {
            background-color: #444; /* Change background color on hover */
            transform: scale(1.05);
        }

        /* Create Post Section */
        .create-post {
            background-color: #1E1E1E;
            padding: 20px;
            border-radius: 10px;
            margin: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }

        .create-post textarea {
            width: 100%;
            background-color: #292929;
            border: 1px solid #444;
            padding: 10px;
            color: white;
            border-radius: 5px;
            resize: none;
            margin-bottom: 10px;
        }

        .create-post button {
            background-color: #007bff;
            color: #ffffff;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .create-post button:hover {
            background-color: #0056b3; /* Darker blue on hover */
        }

        /* Post Styles */
        .post {
            background-color: #1E1E1E;
            padding: 20px;
            border-radius: 10px;
            margin: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
            border: 1px solid #ffffff; /* White border for posts */
        }

        .post-header {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
        }

        .post-header h2 {
            margin: 0;
            font-size: 16px;
            color: #e0e0e0;
        }

        .post-body {
            margin-top: 10px;
        }

        .post-body p {
            font-size: 14px;
            color: #b8b8b8;
        }

        /* Reaction Section */
        .reactions {
            display: flex;
            justify-content: flex-start;
            margin-top: 10px;
        }

        .reaction-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 3px; /* Smaller size for buttons */
            border-radius: 5px;
            margin-right: 10px;
            cursor: pointer;
            background-color: #292929;
            width: 25px; /* Small width for buttons */
            height: 25px; /* Small height for buttons */
            border: 1px solid #555;
            transition: background-color 0.3s, transform 0.3s;
        }

        .reaction-btn:hover {
            background-color: #444;
            transform: scale(1.1);
        }

        .reaction-btn i {
            color: #ffffff;
            font-size: 14px; /* Icon size */
        }

        /* Footer for each post */
        .post-footer {
            display: flex;
            justify-content: space-between;
            margin-top: 15px;
            font-size: 12px;
            color: #777;
        }
    </style>
</head>
<body>

    <!-- Header -->
    <div class="header">
        <button>🏠 Home</button>
        
        <button>👥 Friends</button>
        
        <button>📩 Barta</button>
        
        <button>🔔 notificat</button>
    </div>

    <!-- Create Post Section -->
    <div class="create-post">
        <textarea rows="3" placeholder="What's on your mind?"></textarea>
        <button type="button">Post</button>
    </div>

    <!-- Posts -->
    <!-- Post 1 -->
    <div class="post">
        <div class="post-header">
            <h2>Manik Mia</h2>
        </div>
        <div class="post-body">
            <p>Welcome to our unique social media platform! Enjoy the experience.</p>
        </div>
        <div class="reactions">
            <div class="reaction-btn like-btn">
                <i>👍</i>
            </div>
            <div class="reaction-btn comment-btn">
                <i>💬</i>
            </div>
            <div class="reaction-btn share-btn">
                <i>🔗</i>
            </div>
        </div>
        <div class="post-footer">
            <span>Liked by 120 people</span>
            <span>5 comments</span>
        </div>
    </div>

    <!-- Post 2 -->
    <div class="post">
        <div class="post-header">
            <h2>Shakib Al Hasan</h2>
        </div>
        <div class="post-body">
            <p>This design is fantastic! The colors and layout are so fresh and unique.</p>
        </div>
        <div class="reactions">
            <div class="reaction-btn like-btn">
                <i>👍</i>
            </div>
            <div class="reaction-btn comment-btn">
                <i>💬</i>
            </div>
            <div class="reaction-btn share-btn">
                <i>🔗</i>
            </div>
        </div>
        <div class="post-footer">
            <span>Liked by 89 people</span>
            <span>12 comments</span>
        </div>
    </div>

    <!-- Post 3 -->
    <div class="post">
        <div class="post-header">
            <h2>Pori Moni</h2>
        </div>
        <div class="post-body">
            <p>Learning new things every day! #motivation</p>
        </div>
        <div class="reactions">
            <div class="reaction-btn like-btn">
                <i>👍</i>
            </div>
            <div class="reaction-btn comment-btn">
                <i>💬</i>
            </div>
            <div class="reaction-btn share-btn">
                <i>🔗</i>
            </div>
        </div>
        <div class="post-footer">
            <span>Liked by 75 people</span>
            <span>3 comments</span>
        </div>
    </div>

    <!-- Post 4 -->
    <div class="post">
        <div class="post-header">
            <h2>Miya Khalifa</h2>
        </div>
        <div class="post-body">
            <p>Excited to share my thoughts here! #newbeginnings</p>
        </div>
        <div class="reactions">
            <div class="reaction-btn like-btn">
                <i>👍</i>
            </div>
            <div class="reaction-btn comment-btn">
                <i>💬</i>
            </div>
            <div class="reaction-btn share-btn">
                <i>🔗</i>
            </div>
        </div>
        <div class="post-footer">
            <span>Liked by 45 people</span>
            <span>10 comments</span>
        </div>
    </div>

    <!-- Post 5 -->
    <div class="post">
        <div class="post-header">
            <h2>Hero Alom</h2>
        </div>
        <div class="post-body">
            <p>Let's create a positive community together! #love</p>
        </div>
        <div class="reactions">
            <div class="reaction-btn like-btn">
                <i>👍</i>
            </div>
            <div class="reaction-btn comment-btn">
                <i>💬</i>
            </div>
            <div class="reaction-btn share-btn">
                <i>🔗</i>
            </div>
        </div>
        <div class="post
        
