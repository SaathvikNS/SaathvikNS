## 👋 Hi there! I'm Saathvik N S

I'm a passionate and rapid learner currently pursuing an MCA and excited to dive into the world of technology. With a solid foundation and above-intermediate skills in Python, C, C++, MERN stack, HTML, CSS and JavaScript, I'm always on the lookout for new challenges and opportunities to grow.

### 🔧 Skills & Proficiency:

Programming Languages: Above intermediate in Python, C, C++, JavaScript, HTML, CSS and MERN stack.
Web Technologies: Lower intermediate in Java and proficient at using Linux environments.
Learning Agility: Capable of mastering new skills and technologies within a matter of days.

### 🎓 Education:

MCA 1st Year Student: Currently studying in my first year, eager to apply and expand my knowledge in various tech domains.

### 🌟 Interests & Goals:

Keenly interested in exploring a wide range of opportunities in technology.
Dedicated to developing innovative projects and contributing to exciting tech developments.

# Learning Motivation Function

This motivational function is designed to help programmers stay motivated based on their skill level and learning speed. Whether you're a beginner or an advanced coder, this function provides a fun emoji and tailored advice to keep you inspired.

## Usage

Call the `learning_motivation` function with your task and skill level to receive a custom motivational message.

```python
def learning_motivation(task: str, skill_level: str = 'intermediate') -> str:
    """
    A function to provide motivational messages and advice based on skill level and learning speed.

    Args:
    - task (str): The programming task to execute.
    - skill_level (str): Your current skill level. Default is 'intermediate'.

    Returns:
    - str: A motivational message and advice.
    """
    emojis = {
        'beginner': '🌱',
        'intermediate': '🚀',
        'advanced': '🌟',
        'expert': '🏆'
    }

    advice = {
        'beginner': "Keep learning and experimenting—every step counts!",
        'intermediate': "You're on the right track! Continue to challenge yourself and expand your knowledge.",
        'advanced': "Great progress! Focus on refining your skills and exploring new technologies.",
        'expert': "Exceptional work! Share your knowledge and mentor others while continuing to innovate."
    }

    if skill_level not in emojis:
        return "Invalid skill level! Please choose between 'beginner', 'intermediate', 'advanced', or 'expert'."

    return (f"Task: {task} {emojis[skill_level]}. "
            f"Advice: {advice[skill_level]} Keep up the great work and continue learning!")
