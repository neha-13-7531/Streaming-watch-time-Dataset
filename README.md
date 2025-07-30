## 📊 Streaming Watchtime Analysis
This project analyzes user watchtime data across various streaming platforms to uncover insights about viewer behavior, platform engagement, and content popularity.

## 📌 Summary
This project analyzes a streaming watchtime dataset to uncover trends in user behavior across platforms like Netflix, Hulu, and Amazon Prime. Using Python (Pandas, NumPy, Seaborn, Matplotlib), the notebook performs data cleaning, exploratory analysis, and visualizations.

## 🧾 Dataset Features
- **user_id**	:	Unique identifier for each user
- **platform** : Name of the streaming platform (e.g., Netflix, Hulu)
- **watch_time_minutes** : Total time user spent watching content (in minutes)
- **genre** : Genre of the content watched (e.g., Drama, Horror)
- **date** : Date when the content was watched
- **device** : 	Device used to watch content (e.g., Smart TV, Mobile)
- **location** : Geographic location of the user
- **completion_rate** : Percentage of content watched (0 to 100%)
- **watch_category**:	Category of viewing time (e.g., Short, Long sessions)

🧰 Tools and Libraries Used
- Pandas – Data manipulation and analysis
- NumPy – Mathematical operations
- Matplotlib & Seaborn – Data visualization
- Jupyter Notebook – Interactive analysis environment

🔍 Steps Perform
1. 📥 Data Import
- Loaded dataset using pandas in Jupyter Notebook.

2. 🧹 Data Cleaning
- Converted date columns to datetime format.
- Drop the user_id column.

3. 📊 Exploratory Data Analysis (EDA)
- count the each values in device column.(Smart TV :870 , Gaming Console 853)
- Average completion rate per platform.
- Sorted content by completion rate in ascending order.

4. 📈 Data Visualization
- A histogram was used to understand the distribution of the completion_rate feature.
- Histogram : used for data distribution of watch_time_minutes.
- Heatmap : Correlation between  watch_time_minutes and completion rate.
- Boxplot : To find outlier in watch_time_minutes and completion rate columns.(there is no outlier present in both columns)
- Countplot : Frequency of categorical values (e.g., platform, device)

  💡 Recommendations
  1. 📱 Smart TV & Tablet Optimization
Insight: Users accessing content via Smart TVs and Tablets have significantly higher average watch times compared to Mobile or Web.
✅ Recommendation: Focus feature development (e.g., autoplay, resume watching, personalized banners) on Smart TV and Tablet platforms to retain long-viewing users.

2. 📉 Platform Completion Rate Disparities
Insight: Platforms like Netflix have noticeably higher completion rates, whereas others like mobile web or browser-based apps show lower values.
✅ Recommendation: Audit low-performing platforms for UX issues (buffering, layout, navigation). Consider user interviews or session recordings to understand drop-off points.

3. 😱 High Engagement with Long Horror Content
Insight: Users show high watch time on content where genre = Horror and watch_category = Long.
✅ Recommendation: Invest in and promote long-form horror content. Offer content bundles (e.g., horror marathons, limited-time horror series) to boost retention.

4. 🕐 Short Content Drop-Off
Insight: Some short content (<5 minutes) still has low completion rates, possibly due to poor intros, irrelevant recommendations, or lack of a hook.
✅ Recommendation: Introduce “Auto-next” functionality or group shorts into a playlist to maintain user flow.

5. 💻 Desktop/Web Viewer Behavior
Insight: Desktop/web users have moderate watch time and completion rates — possibly due to distractions or multitasking.
✅ Recommendation: Use visual cues like a “Continue Watching” bar and resume-from-last-time modals. Run user retention experiments (e.g., sticky headers, compact layouts) on web platforms.

